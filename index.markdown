---
layout: page
title: Welcome to The Affirmatron
---

#### _The World's First Fully Automated Affirmation Machine_

We believe that positive affirmations can have a powerful impact on our lives. By consistently repeating positive thoughts and beliefs, we can cultivate a more optimistic and confident mindset. You tell us your affirmation and we repeat it thousands of times to help make it come true! We believe that everyone deserves to feel confident, empowered, and inspired to live their best life.

### Today's Featured Affirmation

<p>Your affirmation for today is: <i><span id="affirmation"></span></i></p>

### Submit An Affirmation for Processing
Your affirmation will be submitted to our servers and repeated to the universe, 1000x within a week!

{% include contact-form.html %}

## Resources

Check out our resources page for more information about the power of affirmations and how to incorporate them into your daily routine.

Thank you for visiting our site! We hope that our affirmations help you cultivate a positive mindset and live your best life.

<script>
const affirmations = {{ site.data.affirmations | jsonify }};
const randomIndex = Math.floor(Math.random() * affirmations.length);
document.getElementById("affirmation").innerHTML = affirmations[randomIndex];
</script>
