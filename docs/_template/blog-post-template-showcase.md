---
layout: post
title: "Template: Example Blog Post"
date: 2026-04-21 09:00:00 -0700
categories: [research-computing]
tags: [template, onboarding, hpc]
cover_image: /images/cmc.webp
author: "Your Name"
excerpt: "A reusable post template that demonstrates headings, lists, images, tables, code blocks, and links."
---

## Summary

Hello! Use this template as a starting point for new onboarding blog posts.
Replace placeholder text with your content and keep only the sections you need.

## Example List

- State the core problem or topic in one sentence.
- Explain who is affected and why it matters.
- Share the outcome, workaround, or recommendation.

## Example Images

Use images to clarify steps or provide visual context. 

*Tip: Store images under `docs/images/` and reference with `{{ "/images/your-file.png" | relative_url }}`.*

### Default Image
![Default Image example]({{ "/images/HPC_Cluster.png" | relative_url }})

### 67% Width Centered Image
![67% width centered image example]({{ "/images/HPC_Cluster.png" | relative_url }}){: .img-67-centered }

### 33% Width Centered Image
![33% width centered image example]({{ "/images/HPC_Cluster.png" | relative_url }}){: .img-33-centered }

### Left-Wrapped Image
![Left wrapped image example]({{ "/images/HPC_Cluster.png" | relative_url }}){: .img-left-wrap }
Text can wrap around the right side of this image.

## Example Table

Use tables for quick comparisons, requirements, or checklists.

| Item | Description | Status |
|---|---|---|
| Account Access | Confirm account is active and credentials work | Required |
| SSH Key | Generate and upload public key | Required |
| Test Login | Verify terminal or OOD shell access | Recommended |
| Follow-up | Share unresolved issues with support | Optional |

## Step-by-Step Section

1. Add background and pre-requisites.
2. Provide a numbered workflow.
3. Include screenshots at key steps.
4. Add verification steps at the end.

## Example Command Block

```bash
ssh username@computer
```

## Notes and Variations

- You can add FAQ-style sections using `##` headings.
- You can add links to internal pages and docs.
- You can remove sections that are not relevant.

## References

- [Jekyll Markdown Guide](https://www.markdownguide.org/tools/jekyll/)