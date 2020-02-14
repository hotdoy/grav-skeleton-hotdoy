---
title: 'Modular Form'
content_position: center
margin_top: full
padding_top: none
padding_bottom: none
margin_bottom: none
role: default
limit_reveal: '0'
process:
    markdown: true
    twig: true
align: left
width: tight
margin: top
padding: none
display_title: '0'
form:
    name: demo-form-modular
    classes: ajax-form
    action: /home
    fields:
        -
            name: email
            label: Email
            placeholder: email@email.com
            type: email
            validate:
                required: true
        -
            name: name
            label: Name
            placeholder: 'Bob Morane'
            type: text
        -
            name: message
            type: textarea
            label: Message
            placeholder: 'Write something nice'
    buttons:
        -
            type: submit
            value: Submit
    process:
        -
            email:
                from: '{{ config.plugins.email.from }}'
                to:
                    - '{{ config.plugins.email.to }}'
                subject: 'CONTACT - {{ form.value.email|e }}'
                body: '{% include ''forms/data.html.twig'' %}'
        -
            email:
                from: '{{ config.plugins.email.from }}'
                to:
                    - '{{ form.value.email }}'
                subject: 'Message received! 👌'
                body: '{% include "emails/demo-confirmation.html.twig" %}'
        -
            reset: true
        -
            message: 'Horray! You just submitted a form trough a modular!'
---

[tight]
## Questions, issues or requests?
Hit me up!

{% include "forms/form.html.twig" with { form: forms('demo-form-modular') } %}
[/tight]

