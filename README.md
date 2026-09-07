# https://bestaicertifications.com/
22 AI certifications scored on six factors, with hours, level and coding needs,education    online learning    artificial intelligence    data analytics careers      deep learning      computer science           tabular
### About this dataset

An independent editorial dataset covering **22 AI certifications and course tracks** from Coursera, DataCamp, Udemy, Google, IBM, DeepLearning.AI/Stanford, Google Cloud and Vanderbilt.

Unlike a scrape of provider marketing pages, every row here carries a **hand-set editorial rating** on a published six-factor methodology, plus the fields people actually decide on: total study hours, difficulty level, and whether the course requires coding.

Maintained by [BestAICertifications.com](https://bestaicertifications.com/ai-certification-statistics/) and refreshed when a tracked programme changes materially. Last updated 2026-09-05.

### Columns

| field | description |
|---|---|
| `id` | Stable identifier for the certification |
| `name` | Programme name as the provider publishes it |
| `provider` | DataCamp (12), Udemy (4), and one each from Google, Google Cloud, IBM, DeepLearning.AI, DeepLearning.AI & Stanford, Vanderbilt |
| `level` | Editorial difficulty: Beginner (9), Intermediate (12), Advanced (1) |
| `typicalHours` | Total study hours, 1.5 to 174. `null` where no provider figure is held |
| `codingRequired` | `none` (6), `light Python` (1), `Python` (10), `null` where we have not read the syllabus first-hand (5) |
| `editorialRating` | Our score, 1–5. Range 4.1–4.9, mean 4.51 |
| `ratingScale` | Always `"1-5"` |
| `reviewUrl` | Link to our full written review, where one exists (7 of 22) |
| `enrollUrl` | The provider's own public course page |

### Three things worth knowing before you use it

**1. `editorialRating` is an opinion score, not a user average.** It is set on six factors — curriculum currency, completion realism, skill value, employer recognition, cost & value, and salary impact — weighted hardest toward the first two. It is not an average of student reviews and not a survey of employers. Describe it that way if you cite it.

**2. `typicalHours` is a duration, not a pace.** Providers advertise things like "6 months at 7 hours a week", which is a *pace* and is not comparable between providers. This column is that pace multiplied out to a single total-hours figure, which is the only pace-independent form. `null` means no provider figure is held, never zero.

**3. Nulls are honest, not missing.** A course we do not score is absent from this file entirely rather than given an invented rating, and `codingRequired` is `null` for the five programmes whose syllabus we have not read first-hand. Nothing here is imputed.

### Ideas for things to do with it

- Does a higher price buy a better-rated course? Join `provider` against public pricing.
- Do no-coding certifications cluster at the beginner end, or is that an assumption? (6 of 22 need no programming at all.)
- Hours vs rating: is longer better? The range runs 1.5 to 174 hours.
- Build a recommender: level + coding tolerance + hours available → a shortlist.

### Licence and citation

Published under **CC BY 4.0** — free to reuse, including commercially, with attribution.

> Nisar, Rohail. "AI Certification Dataset." BestAICertifications.com, 2026,
> https://bestaicertifications.com/ai-certification-statistics/

The canonical, always-current version lives at
**https://bestaicertifications.com/ai-certification-statistics/dataset.json**
alongside the full methodology at https://bestaicertifications.com/about/
