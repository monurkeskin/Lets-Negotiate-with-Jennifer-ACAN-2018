# Method and evidence

Associated paper: [Let's Negotiate with Jennifer! Towards a Speech-Based Human-Robot Negotiation](https://doi.org/10.1007/978-981-15-5869-6_1).

## Scientific contract

Two quadratic TSBT bounds, AC-Next, notification/offer/response stages and prioritized mood rules.

Five-minute practice, ten-minute eight-item island negotiation, 30-point target; bids describe the human share.

The machine-readable [paper map](paper-map.json) links selected manuscript labels,
source hashes and locations to implementation, independent tests, configurations
and result targets. Only the selected active LaTeX entry was used. Manuscript
working files, inactive drafts and reviewer correspondence are not redistributed.


## Interaction and presentation

The Ready → human offer → agent response → Accept/Reject → Ready handshake is
implemented. Notifications and rejections are protocol events, not formal bids.
A stale offer reference cannot reject a newer offer. The human-share perspective
is the same in structured input, text parsing, spoken proposal and utility tests.

The paper mood priority is selectable per condition. The templates expose an
illustrative warning fraction `.8` and BABT mild multiplier `.95`; numerical
historical confirmation and the original argument/gesture corpus are preflight
gaps. Generated plain-language proposals do not claim to recreate those corpora.
Gesture-disabled conditions suppress gesture commands while retaining speech.

## Utility, targets and game scores

A bid always states the human share. Agent utility uses the complementary allocation.
Utility is computed at full precision; rendering multiplies by 100 for display.
A target score is distinct from a reservation constraint. In the fruit papers,
a human agreement below 40 points is permitted but earns zero game points;
raw utility and game payoff remain separate logged fields. The Jennifer papers'
30-point goal is not silently turned into a prohibition on lower agreements.
The short Solver and Appearance examples do not claim those fruit reward rules.

## Remaining evidence gaps

- Original three-issue practice domain and point tables.
- Original questionnaire, arguments, gesture corpus and recording assets.
- Numerical warning and mood thresholds with historical provenance.
- Permitted session-level human outcomes and analysis records.

Unknown inputs are not filled with simulated participants or invented historical
constants. The existing templates are inspectable, but their published-protocol
preflight prevents starting before required evidence is supplied and reviewed.
A custom study has its own declared configuration and cannot inherit a reproduction
claim merely by using the same strategy name.

## Relationship to the research series

The later journal article expands the strategy and experimental design; its conditions cannot be pooled with this study.

The common engine owns utility, lifecycle, logs, GUI, shared methods and device
contracts. This repository owns paper-specific profiles, protocol choices, analysis
rules, reproduction targets and tests. [framework.json](framework.json) pins the
engine; [NOTICE](NOTICE) preserves original source attribution.

## Social reaction and agreement thresholds

Protocol revision 3 in release 2.1.0 records `offended_threshold: 0.3` separately from
the preference reservation. This restores the low-offer social reaction while
keeping offers below that social threshold legally negotiable. The value follows
the historical Jennifer mood implementation; it is not an estimated optimum.
The maintained warning fraction and mild multiplier are unchanged.

Older journals without this field retain their recorded reservation-based mood
behavior on replay. Release 2.1.0 pins the matching engine; the archived 2.0.0
configurations retain their previous behavior.

## Retained presentation choices

The maintained warning fraction is .8 and the mild multiplier is .95. The
inspected historical controller uses a .7 warning; the historical BABT wrapper
uses .9 for its mild multiplier. The author accepted retaining the maintained
values, so these are explicit choices rather than recovered historical constants.
