# Trust-risk gap analysis: Snapchat, Facebook and WhatsApp

Analysis pipeline for my CM3203 final year project at Cardiff University (BSc Computer Science with Security and Forensics). The project looks at the gap between how much people trust a social platform and how well they can recognise grooming or abusive behaviour on it.

The notebook loads a survey export, cleans it, builds composite trust and risk scores per platform, and produces six charts.

## Output

| Figure | Shows |
|---|---|
| `chart1_trust_risk_gap_by_platform.png` | Trust-risk gap per platform |
| `chart2_correlation_heatmap.png` | Correlations between survey measures |
| `chart3_composite_by_background.png` | Composite score by academic background |
| `chart4_trust_vs_stranger_contact.png` | Trust against stranger contact |
| `chart5_composite_by_gender.png` | Composite score by gender |
| `chart6_composite_by_age.png` | Composite score by age range |

All are in `figures/`.

## Run it

```
pip install -r requirements.txt
jupyter notebook analyser.ipynb
```

You need your own `data/survey_responses.csv`. See `data/README.md` for why the original isn't included.

## Notes

`notebook_explanation.txt` walks through every cell in plain English. Question 9 is absent from the survey export, so numbering jumps from Q8 to Q10. That is intentional.

The sample is small (21 responses), so treat the charts as descriptive, not as evidence of population-level effects.
