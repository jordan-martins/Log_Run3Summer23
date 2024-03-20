# Due Diligence
#PPD/Run3Summer23

PPD accidentally found two issues with the 2023 MC Campaigns. In particular, both problems are related to an update in GT (in the non-BPix and BPix Campaigns), understood as needed from AlCa and PdmV. The specific root issue update was the insertion of HCAL conditions set for the yet-to-be-created 2023 MC that will be used for the yet-to-be-processed ReRECO of the 2023 DATA. This update was in the McM on Jan. 15th, 2024.

The total bulk of requests that need to be redone is the following:
- Run3Summer23BPix 
  - 801 requests for 848M events submitted/processed
  - [Samples](https://github.com/jordan-martins/Log_Run3Summer23/blob/main/Run3Summer23BPixDR_/bpix_campaing.md) that are being invalidated and resubmitted
- Run3Summer23
  - 789 requests for 1.425B events submitted/processed
  - [Samples](https://github.com/jordan-martins/Log_Run3Summer23/blob/main/Run3Summer23_/non_bpix.md) that are being invalidated and resubmitted

Extended McM *downtime* is because this operation, in addition to being highly heavy on DB operations, will take approximately 2.3 days to be concluded.

Those 2.2B events will get high priority >110k  (Block 0 - PPD Operations), with POG samples for SF slightly higher than the PAG ones. All the progress can be monitored in GrASP via the tag **PPD_OPS_GT**. We expect to recover this backlog between 2 and 3 weeks at the cost of pausing the ongoing workflows that would be in lower priority.

In more technical terms, the Run3Summer23BPix MC Campaign should have the ￼`130X_mcRun3_2023_realistic_postBPix_v[1,2,6]`￼, while the Run3Summer23 should have `130X_mcRun3_2023_realistic_v[14,15]`.
