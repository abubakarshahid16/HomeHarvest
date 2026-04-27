# Demo Video Guide

This repo does not include a real recorded video yet.

That is normal. A proper demo should be recorded against a live run so viewers can trust what they see.

## Recommended video length

- `2 to 4 minutes`

## What to record

### 1. Problem statement

Open the README and explain:

- why manual listing research is slow
- why structured property data matters
- who benefits from HomeHarvest

### 2. Quick code example

Show a small script like:

```python
from homeharvest import scrape_property

properties = scrape_property(
    location="San Diego, CA",
    listing_type="sold",
    past_days=30,
)

print(properties.head())
```

### 3. Filtering example

Show a second example with filters:

```python
properties = scrape_property(
    location="Atlanta, GA",
    listing_type="for_sale",
    beds_min=3,
    price_max=450000,
    sqft_min=1400,
    limit=50,
)
```

### 4. Export example

Show:

```python
properties.to_csv("results.csv", index=False)
```

Then briefly open the CSV so viewers can see the structured output.

### 5. Real-world positioning

End the video by explaining that HomeHarvest can be used for:

- investor market scans
- brokerage research
- comps and deal screening
- downstream analytics pipelines

## Suggested voiceover

You can say:

> HomeHarvest helps turn manual property research into a repeatable Python workflow. Instead of copying listing data by hand, we can search, filter, structure, and export it for analysis in just a few lines of code.

## Where to put the final link

After recording, replace the placeholder Loom link in:

- `README.md`

## Best recording tools

- Loom
- OBS Studio
- YouTube unlisted upload
