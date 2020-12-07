---
layout: page
parent: "Components"
title: "Slider"
shortName: "component__slider"
intro: "The Slider component, also known as a Range Input, allows users to choose an approximate number from a range."
jump_menu: true
title_label: 'May require JavaScript'
---

At its root the Slider component is a native `<input>` form element with an attribute `type` of `range`.

<div class="ds-preview">
  <input class="fsa-slider" id="lorem-range-2229" name="lorem-range-2229" type="range" min="0" max="100" value="30" step="10">
</div>
```html
<input class="fsa-slider" id="lorem-range-2229" name="lorem-range-2229" type="range" min="0" max="100" value="30" step="10">
```

## Variations

### Full-width

<div class="ds-preview">
  <input class="fsa-slider fsa-slider--block" id="lorem-range-4453" name="lorem-range-4453" type="range" min="0" max="100" value="90" step="10">
</div>
```html
<input class="fsa-slider fsa-slider--block" id="lorem-range-4453" name="lorem-range-4453" type="range" min="0" max="100" value="90" step="10">
```

### Disabled

<div class="ds-preview">
  <input class="fsa-slider" id="lorem-range-3309" name="lorem-range-3309" type="range" min="0" max="100" value="40" step="10" disabled="">
</div>
```html
<input class="fsa-slider" id="lorem-range-3309" name="lorem-range-3309" type="range" min="0" max="100" value="40" step="10" disabled="">
```

### Vertical

<div class="ds-preview">
  <div class="fsa-slider-vertical">
    <input class="fsa-slider" id="lorem-range-2229" name="lorem-range-2229" type="range" min="0" max="100" value="30" step="10">
  </div>
</div>
```html
<div class="fsa-slider-vertical">
  <input class="fsa-slider" id="lorem-range-2229" name="lorem-range-2229" type="range" min="0" max="100" value="30" step="10">
</div>
```

### Vertical, Custom Height

<div class="ds-preview">
  <div class="fsa-slider-vertical" style="--slider-vertical-height: 10rem">
    <input class="fsa-slider" id="lorem-range-2229" name="lorem-range-2229" type="range" min="0" max="100" value="60" step="10">
  </div>
</div>
```html
<div class="fsa-slider-vertical" style="--slider-vertical-height: 10rem">
  <input class="fsa-slider" id="lorem-range-2229" name="lorem-range-2229" type="range" min="0" max="100" value="60" step="10">
</div>
```

## Examples

### With output

Combine with [Level]({{ site.baseurl }}layout/level/) layout component to arrange Slider with an `<output>` element (note [JavaScript guidance](#javascript-guidance)).

<div class="ds-preview">
  <div class="fsa-level">
    <span>
      <input class="fsa-slider fsa-slider--block" id="lorem-range-4672" name="lorem-range-4672" type="range" min="0" max="100" value="90" step="10">
    </span>
    <span><output aria-live="polite" id="lorem-range-ouput-6789" name="lorem-range-ouput-6789" for="lorem-range-4672">90</output></span>
  </div>
</div>
```html
<div class="fsa-level">
  <span>
    <input class="fsa-slider fsa-slider--block" id="lorem-range-4672" name="lorem-range-4672" type="range" min="0" max="100" value="90" step="10">
  </span>
  <span><output aria-live="polite" id="lorem-range-ouput-6789" name="lorem-range-ouput-6789" for="lorem-range-4672">90</output></span>
</div>
```

### With output, Full-width

Combine the `fsa-slider--block` variation with [Level]({{ site.baseurl }}layout/level/) to arrange Slider with an `<output>` element (note [JavaScript guidance](#javascript-guidance)).

<div class="ds-preview">
  <div class="fsa-level">
    <span class="fsa-level__item--grow-auto">
      <input class="fsa-slider fsa-slider--block" id="lorem-range-4672" name="lorem-range-4672" type="range" min="0" max="100" value="10" step="10">
    </span>
    <span><output aria-live="polite" id="lorem-range-ouput-6789" name="lorem-range-ouput-6789" for="lorem-range-4672">10</output></span>
  </div>
</div>
```html
<div class="fsa-level">
  <span class="fsa-level__item--grow-auto">
    <input class="fsa-slider fsa-slider--block" id="lorem-range-4672" name="lorem-range-4672" type="range" min="0" max="100" value="10" step="10">
  </span>
  <span><output aria-live="polite" id="lorem-range-ouput-6789" name="lorem-range-ouput-6789" for="lorem-range-4672">10</output></span>
</div>
```

### Within Field component

Nested within a [Form Field]({{ site.baseurl }}components/form-fields/).

<div class="ds-preview">
  <div class="fsa-field">
    <label class="fsa-field__label" for="lorem-range-1234">Label <span class="fsa-field__label-desc">Required</span></label>
    <input class="fsa-slider fsa-field__item" id="lorem-range-1234" name="lorem-range-1234" type="range" min="0" max="10" value="3" step="1">
  </div>
  <div class="fsa-field">
    <label class="fsa-field__label" for="lorem-range-7710">Label <span class="fsa-field__label-desc">Required</span></label>
    <div class="fsa-level">
      <span class="fsa-level__item--grow-auto">
        <input class="fsa-slider fsa-field__item" id="lorem-range-7710" name="lorem-range-7710" type="range" min="0" max="10" value="3" step="1">
      </span>
      <span><output aria-live="polite" id="lorem-range-ouput-7710" name="lorem-range-ouput-7710" for="lorem-range-7710">90</output></span>
    </div>
  </div>
</div>
```html
<div class="fsa-field">
  <label class="fsa-field__label" for="lorem-range-7710">Label <span class="fsa-field__label-desc">Required</span></label>
  <div class="fsa-level">
    <span class="fsa-level__item--grow-auto">
      <input class="fsa-slider fsa-field__item" id="lorem-range-7710" name="lorem-range-7710" type="range" min="0" max="10" value="3" step="1">
    </span>
    <span><output aria-live="polite" id="lorem-range-ouput-7710" name="lorem-range-ouput-7710" for="lorem-range-7710">90</output></span>
  </div>
</div>
```

## Usage

{% capture usage_do %}
* When the range is more important than precision.
    * For instance, it could be more important for a target price selector to communicate where the target price falls within a certain range than the precise dollar amount selected.
* When a relative value is more important than an exact value.
    * For instance, a volume slider is typically more focussed on the relative loudness of the output rather than the specific decibel level.
{% endcapture %}

{% capture usage_dont %}
* When the accuracy of the numeric value entered is important. Consider using number input instead.
* If a precise number should be entered, consider a regular [Text Input]({{ site.baseurl }}components/text-input/) or  [Spinbox]({{ site.baseurl }}components/spinbox/).
* For ranges that are extremely large i.e. 1-1000.
* For ranges that are too small i.e. 1-3.
{% endcapture %}

{% include do-dont.html %}

## General Guidance

* Accepted attributes to describe the Slider `input[type=range]`:
    * `value`: Current value.
    * `min`: Minimum value.
    * `max`: Maximum value.
    * `step`: The granularity the value may be increased or decreased.
* Label the limits of the range.
    * When appropriate, label the ends of the slider with the limits of the range (for example: “0/100”, “small/large” or “less expensive/more expensive”).
* Don’t be too granular. In a range slider, the relative value is more important than the specific value, so set the `step` attribute so it’s not too granular.
    * By setting the `step` attribute to a value of 10-20% of the total range you prevent unnecessary precision and cognitive strain in your users.
    * For example, set `step="10"` in a total range of 100.

## JavaScript Guidance

Some [example implementations](#examples) of this component can pair with an `<output>` element to surface its approximate value to the user, however JavaScript would be required. Below is an example script to reflect the Slider's dynamic updated value:

<div class="ds-preview">
  <div class="fsa-level">
    <input oninput="result.value=a.value" class="fsa-slider" id="a" name="a" type="range" min="0" max="100" value="30" step="10">
    <output aria-live="polite" id="result" name="result" for="a">30</output>
  </div>
</div>

{% include scripts.about.html %}
