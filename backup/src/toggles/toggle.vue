<template>
	<div class="example example-light">

      <div class="row">
        <div class="large-3">
          <label class="switch-light switch-material" onclick="">
            <input type="checkbox">

            <strong>
              Wireless
            </strong>

            <span>
              <span>Off</span>
              <span>On</span>
              <a></a>
            </span>
          </label>
        </div>
      </div>

      <div class="row">
        <div class="large-4">
          <label>View</label>
          <div class="switch-toggle switch-material">
            <input id="e-m1" name="e-m" type="radio" checked="">
            <label for="e-m1" onclick="">Week</label>

            <input id="e-m2" name="e-m" type="radio">
            <label for="e-m2" onclick="">Month</label>

            <input id="e-m3" name="e-m" type="radio">
            <label for="e-m3" onclick="">Year</label>

            <a></a>
          </div>
        </div>
      </div>

    </div>
</template>
<style lang="stylus">
.switch-toggle a, .switch-light span span {
  display: none; }

/* We can't test for a specific feature,
 * so we only target browsers with support for media queries.
 */
@media only screen {
  /* Checkbox
 */
  .switch-light {
    position: relative;
    display: block;
    overflow: hidden;
    /* Outline the toggles when the inputs are focused
  */ }
    .switch-light *, .switch-light *:before, .switch-light *:after {
      box-sizing: border-box; }
    .switch-light a {
      display: block;
      -webkit-transition: all 0.2s ease-out;
      -moz-transition: all 0.2s ease-out;
      transition: all 0.2s ease-out; }
    .switch-light label, .switch-light > span {
      /* breathing room for bootstrap/foundation classes
     */
      line-height: 2em;
      vertical-align: middle; }
    .switch-light input:focus ~ span a, .switch-light input:focus + label {
      outline: 1px dotted #888; }
  /* don't hide the input from screen-readers and keyboard access
 */
  .switch-light input {
    position: absolute;
    opacity: 0;
    z-index: 3; }
  .switch-light input:checked ~ span a {
    right: 0%; }
  /* inherit from label
 */
  .switch-light strong {
    font-weight: inherit; }
  .switch-light > span {
    position: relative;
    overflow: hidden;
    display: block;
    min-height: 2em;
    /* overwrite 3rd party classes padding
   * eg. bootstrap .well
   */
    padding: 0;
    text-align: left; }
  .switch-light span span {
    position: relative;
    z-index: 2;
    display: block;
    float: left;
    width: 50%;
    text-align: center;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none; }
  .switch-light a {
    position: absolute;
    right: 50%;
    top: 0;
    z-index: 1;
    display: block;
    width: 50%;
    height: 100%;
    padding: 0; }
  /* Radio Switch
 */
  .switch-toggle {
    position: relative;
    display: block;
    overflow: hidden;
    /* Outline the toggles when the inputs are focused
  */
    /* For callout panels in foundation
  */
    padding: 0 !important;
    /* 2 items
   */
    /* 3 items
   */
    /* 4 items
   */
    /* 5 items
   */
    /* 6 items
   */ }
    .switch-toggle *, .switch-toggle *:before, .switch-toggle *:after {
      box-sizing: border-box; }
    .switch-toggle a {
      display: block;
      -webkit-transition: all 0.2s ease-out;
      -moz-transition: all 0.2s ease-out;
      transition: all 0.2s ease-out; }
    .switch-toggle label, .switch-toggle > span {
      /* breathing room for bootstrap/foundation classes
     */
      line-height: 2em;
      vertical-align: middle; }
    .switch-toggle input:focus ~ span a, .switch-toggle input:focus + label {
      outline: 1px dotted #888; }
    .switch-toggle input {
      position: absolute;
      left: 0;
      opacity: 0; }
    .switch-toggle input + label {
      position: relative;
      z-index: 2;
      display: block;
      float: left;
      padding: 0 8px;
      margin: 0;
      text-align: center; }
    .switch-toggle a {
      position: absolute;
      top: 0;
      left: 0;
      padding: 0;
      z-index: 1;
      width: 10px;
      height: 100%; }
    .switch-toggle label:nth-child(2):nth-last-child(4), .switch-toggle label:nth-child(2):nth-last-child(4) ~ label, .switch-toggle label:nth-child(2):nth-last-child(4) ~ a {
      width: 50%; }
    .switch-toggle label:nth-child(2):nth-last-child(4) ~ input:checked:nth-child(3) + label ~ a {
      left: 50%; }
    .switch-toggle label:nth-child(2):nth-last-child(6), .switch-toggle label:nth-child(2):nth-last-child(6) ~ label, .switch-toggle label:nth-child(2):nth-last-child(6) ~ a {
      width: 33.33%; }
    .switch-toggle label:nth-child(2):nth-last-child(6) ~ input:checked:nth-child(3) + label ~ a {
      left: 33.33%; }
    .switch-toggle label:nth-child(2):nth-last-child(6) ~ input:checked:nth-child(5) + label ~ a {
      left: 66.66%; }
    .switch-toggle label:nth-child(2):nth-last-child(8), .switch-toggle label:nth-child(2):nth-last-child(8) ~ label, .switch-toggle label:nth-child(2):nth-last-child(8) ~ a {
      width: 25%; }
    .switch-toggle label:nth-child(2):nth-last-child(8) ~ input:checked:nth-child(3) + label ~ a {
      left: 25%; }
    .switch-toggle label:nth-child(2):nth-last-child(8) ~ input:checked:nth-child(5) + label ~ a {
      left: 50%; }
    .switch-toggle label:nth-child(2):nth-last-child(8) ~ input:checked:nth-child(7) + label ~ a {
      left: 75%; }
    .switch-toggle label:nth-child(2):nth-last-child(10), .switch-toggle label:nth-child(2):nth-last-child(10) ~ label, .switch-toggle label:nth-child(2):nth-last-child(10) ~ a {
      width: 20%; }
    .switch-toggle label:nth-child(2):nth-last-child(10) ~ input:checked:nth-child(3) + label ~ a {
      left: 20%; }
    .switch-toggle label:nth-child(2):nth-last-child(10) ~ input:checked:nth-child(5) + label ~ a {
      left: 40%; }
    .switch-toggle label:nth-child(2):nth-last-child(10) ~ input:checked:nth-child(7) + label ~ a {
      left: 60%; }
    .switch-toggle label:nth-child(2):nth-last-child(10) ~ input:checked:nth-child(9) + label ~ a {
      left: 80%; }
    .switch-toggle label:nth-child(2):nth-last-child(12), .switch-toggle label:nth-child(2):nth-last-child(12) ~ label, .switch-toggle label:nth-child(2):nth-last-child(12) ~ a {
      width: 16.6%; }
    .switch-toggle label:nth-child(2):nth-last-child(12) ~ input:checked:nth-child(3) + label ~ a {
      left: 16.6%; }
    .switch-toggle label:nth-child(2):nth-last-child(12) ~ input:checked:nth-child(5) + label ~ a {
      left: 33.2%; }
    .switch-toggle label:nth-child(2):nth-last-child(12) ~ input:checked:nth-child(7) + label ~ a {
      left: 49.8%; }
    .switch-toggle label:nth-child(2):nth-last-child(12) ~ input:checked:nth-child(9) + label ~ a {
      left: 66.4%; }
    .switch-toggle label:nth-child(2):nth-last-child(12) ~ input:checked:nth-child(11) + label ~ a {
      left: 83%; }
      //THEME
   .switch-light.switch-material a {
    top: -3px;
    width: 28px;
    height: 28px;
    border-radius: 50%;
    background: #fafafa;
    box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 3px 2px -2px rgba(0, 0, 0, 0.2), 0 2px 4px 0 rgba(0, 0, 0, 0.12);
    -webkit-transition: right .28s cubic-bezier(.4, 0, .2, 1);
    -moz-transition: right .28s cubic-bezier(.4, 0, .2, 1);
    transition: right .28s cubic-bezier(.4, 0, .2, 1); }
  .switch-material.switch-light {
    overflow: visible; }
    .switch-material.switch-light::after {
      clear: both;
      content: "";
      display: table; }
  .switch-material.switch-light > span {
    overflow: visible;
    position: relative;
    top: 3px;
    width: 52px;
    height: 24px;
    min-height: auto;
    border-radius: 16px;
    background: rgba(0, 0, 0, 0.26); }
  .switch-material.switch-light span span {
    position: absolute;
    clip: rect(0 0 0 0); }
  .switch-material.switch-light input:checked ~ span a {
    right: 0;
    background: #3f51b5;
    box-shadow: 0 3px 4px 0 rgba(0, 0, 0, 0.14), 0 3px 3px -2px rgba(0, 0, 0, 0.2), 0 1px 6px 0 rgba(0, 0, 0, 0.12); }
  .switch-material.switch-light input:checked ~ span {
    background: rgba(63, 81, 181, 0.5); }
  /* switch-toggle
 */
  .switch-toggle.switch-material {
    overflow: visible; }
    .switch-toggle.switch-material::after {
      clear: both;
      content: "";
      display: table; }
  .switch-toggle.switch-material a {
    top: 48%;
    width: 6px !important;
    height: 6px;
    margin-left: 4px;
    background: #3f51b5;
    border-radius: 100%;
    -webkit-transform: translateY(-50%);
    -moz-transform: translateY(-50%);
    -ms-transform: translateY(-50%);
    -o-transform: translateY(-50%);
    transform: translateY(-50%);
    -webkit-transition: -webkit-transform 0.4s ease-in;
    -moz-transition: -moz-transform 0.4s ease-in;
    transition: transform 0.4s ease-in; }
  .switch-toggle.switch-material label {
    color: rgba(0, 0, 0, 0.54);
    font-size: 1em; }
  .switch-toggle.switch-material label:before {
    content: '';
    position: absolute;
    top: 48%;
    left: 0;
    display: block;
    width: 14px;
    height: 14px;
    border-radius: 100%;
    border: 2px solid rgba(0, 0, 0, 0.54);
    -webkit-transform: translateY(-50%);
    -moz-transform: translateY(-50%);
    -ms-transform: translateY(-50%);
    -o-transform: translateY(-50%);
    transform: translateY(-50%); }
  .switch-toggle.switch-material input:checked + label:before {
    border-color: #3f51b5; }
  /* ripple
 */
  .switch-light.switch-material > span:before, .switch-light.switch-material > span:after, .switch-toggle.switch-material label:after {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    z-index: 3;
    display: block;
    width: 64px;
    height: 64px;
    border-radius: 100%;
    background: #3f51b5;
    opacity: .4;
    margin-left: -20px;
    margin-top: -20px;
    -webkit-transform: scale(0);
    -moz-transform: scale(0);
    -ms-transform: scale(0);
    -o-transform: scale(0);
    transform: scale(0);
    -webkit-transition: opacity .4s ease-in;
    -moz-transition: opacity .4s ease-in;
    transition: opacity .4s ease-in; }
  .switch-light.switch-material > span:after {
    left: auto;
    right: 0;
    margin-left: 0;
    margin-right: -20px; }
  .switch-toggle.switch-material label:after {
    width: 52px;
    height: 52px;
    margin-top: -12px; }
  @-webkit-keyframes materialRipple {
    0% {
      -webkit-transform: scale(0); }

    20% {
      -webkit-transform: scale(1); }

    100% {
      opacity: 0;
      -webkit-transform: scale(1); } }

  @-moz-keyframes materialRipple {
    0% {
      -moz-transform: scale(0); }

    20% {
      -moz-transform: scale(1); }

    100% {
      opacity: 0;
      -moz-transform: scale(1); } }

  @keyframes materialRipple {
    0% {
      -webkit-transform: scale(0);
      -moz-transform: scale(0);
      -ms-transform: scale(0);
      -o-transform: scale(0);
      transform: scale(0); }

    20% {
      -webkit-transform: scale(1);
      -moz-transform: scale(1);
      -ms-transform: scale(1);
      -o-transform: scale(1);
      transform: scale(1); }

    100% {
      opacity: 0;
      -webkit-transform: scale(1);
      -moz-transform: scale(1);
      -ms-transform: scale(1);
      -o-transform: scale(1);
      transform: scale(1); } }

  .switch-material.switch-light input:not(:checked) ~ span:after, .switch-material.switch-light input:checked ~ span:before, .switch-toggle.switch-material input:checked + label:after {
    -webkit-animation: materialRipple .4s ease-in;
    -moz-animation: materialRipple .4s ease-in;
    animation: materialRipple .4s ease-in; }
  /* trick to prevent the default checked ripple animation from showing
 * when the page loads.
 * the ripples are hidden by default, and shown only when the input is focused.
 */
  .switch-light.switch-material.switch-light input ~ span:before, .switch-light.switch-material.switch-light input ~ span:after, .switch-material.switch-toggle input + label:after {
    visibility: hidden; }
  .switch-light.switch-material.switch-light input:focus:checked ~ span:before, .switch-light.switch-material.switch-light input:focus:not(:checked) ~ span:after, .switch-material.switch-toggle input:focus:checked + label:after {
    visibility: visible; } }

/* Bugfix for older Webkit, including mobile Webkit. Adapted from
 * http://css-tricks.com/webkit-sibling-bug/
 */
@media only screen and (-webkit-max-device-pixel-ratio: 2) and (max-device-width: 1280px) {
  .switch-light, .switch-toggle {
    -webkit-animation: webkitSiblingBugfix infinite 1s; } }

@-webkit-keyframes webkitSiblingBugfix {
  from {
    -webkit-transform: translate3d(0, 0, 0); }

  to {
    -webkit-transform: translate3d(0, 0, 0); } }
     
</style>