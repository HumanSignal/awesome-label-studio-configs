# Two-Level Text Classification

This labeling config lets you assign a **sentiment** (Positive, Negative, or Neutral) to X / Twitter post. 
After picking a sentiment, a second-level classification appears to categorize the text as _Descriptive_, _Emotional_, _Mixed_, _Ambigous_, or _Sarcams_. 
The labeling interface is styled to look like a X / Twitter post."

---

## Preview

![two-level-classification-preview](./preview/two-level-classification-of-x-twitter-posts.gif)

---

## Author & Contributors

- **Author**: [@luarmr](https://github.com/luarmr)
- **Contributors**:
  - [@bmartel](https://github.com/bmartel)
  - [@redeipirati](https://github.com/redeipirati)

---

## Special Instructions

- **Conditional Choices**: The second set of choices (other-props) only appears after selecting a sentiment.

This is done with:

```xml
visibleWhen="choice-selected"
whenTagName="sentiment"
```

---

## More Info

For general usage and installation instructions, see the main
[README](../../README.md) of this repository.
If you have any feedback or suggestions, open a PR or issue on GitHub!
