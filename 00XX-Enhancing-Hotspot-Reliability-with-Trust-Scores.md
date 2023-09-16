# HIP: Enhancing Hotspot Reliability with Trust Scores

**Author(s):** Hans Arndt

## Summary

This HIP proposes a trust scoring system for hotspots to enhance their position and coverage reliability within the Helium network. Trust scores, ranging from 0 to 1, determine a hotspot's qualification for Hex Boosting participation. This document outlines the mechanisms to achieve and maintain these scores.

## Motivation

As the Helium network expands, there's a pronounced need for mechanisms to authenticate hotspot validity. This proposal aims to:

- Solidify hotspot location authenticity.
- Complement the existing Skyhook WiFi verification.
- Provide a consistent measure to evaluate hotspot reliability.

## Stakeholders

- **Hotspot Owners**: Need to align with the criteria for optimal trust scores.
- **Secure Mapper Providers (e.g., NOVA)**: Produce devices enhancing hotspot validation.
- **Hex Boosting Participants**: Depend on trust scores for reward allocations.
- **Helium Network Users**: Require a reliable network anchored by authenticated hotspots.

## Detailed Explanation

1. **Initialization**: All hotspots will start with a trust score of 0 upon implementation.
2. **Skyhook WiFi Verification**: Hotspots can raise their trust score by 0.25 by validating their position through Skyhook WiFi.
3. **Secure Mapper Validation**: Hotspots can obtain an additional 0.25 for validation by a Secure Mapper from NOVA. Each unique Secure Mapper contributes a separate 0.25. However, one Mapper can only revalidate a hotspot once every 90 days. This revalidation supersedes the previous 0.25 score from that Mapper.
4. **Hex Boosting Eligibility**: While a trust score nearing 1 implies a highly credible hotspot, the the threshold to participate in Hex Boosting is 0.5.


## Unresolved Questions
- How can we verify and validate Secure Mappers are from unique parties?
- How can hotspots challenge their trust scores or findings from a Secure Mapper?

## Deployment Impact

Current hotspots will have an initial trust score of 0, marking them ineligible for Hex Boosting. Owners should undergo the stipulated processes to enhance their scores. Educating hotspot owners about this new system becomes imperative to its successful rollout.

