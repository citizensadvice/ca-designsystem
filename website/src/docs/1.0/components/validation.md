---
layout: docs
title: Validation
---

# Validation

Form validation helps us to ensure that users fill out forms in the correct format, making sure that submitted data will work successfully with our applications.

{% capture example %}
<fieldset class="c-fieldset">
    <label class="c-label" for="postcode">
        What's your postcode?
    </label>
    <span class="c-label__metainfo">
        For example: SW1A 2AA
    </span>
    <div class="c-input">
        <input 
        id="postcode" 
        type="text" 
        name="postcode" 
        required />
    </div>
    <label class="input--error" for="postcode">
        Please enter a valid postcode
    </label>
</fieldset>
{% endcapture %}
{% include example.html content=example %}

{% capture snippet %}

<fieldset class="c-fieldset">
    <label class="c-label" for="postcode">
        What's your postcode?
    </label>
    <span class="c-label__metainfo">
        For example: SW1A 2AA
    </span>
    <div class="c-input">
        <input 
        id="postcode" 
        type="text" 
        name="postcode"
        pattern="[a-z]{1,15}"/>
    </div>
    <label class="input--error" for="postcode">
        Please enter a valid postcode
    </label>
</fieldset>
{% endcapture %}
{% include snippet.html content=snippet %}