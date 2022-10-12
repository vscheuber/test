# AA-Login :white_check_mark: enabled, :red_circle: custom, :yellow_circle: premium
`Authentication`, `Social Authentication`, `Adaptive`, `Autonomous Access`
Autonomous Access Login
## Inner Tree Dependencies (3)
- AA-Login
  - iSocialLogin
  - iAA-LoginRisk
    - DevicePrint
    - MFAAutoSelect
      - MFAWithEmailOTP
      - MFAWithVoiceOTP
      - MFAWithSMSOTP
    - iAA-FraudRisk
  - ProgressiveProfile
## Node Types (9)
| Count | Type | Classification |
| -----:| ---- | -------------- |
| 3 | InnerTreeEvaluatorNode | :red_circle: custom |
| 1 | IncrementLoginCountNode | :red_circle: custom |
| 2 | ScriptedDecisionNode | :red_circle: custom |
| 2 | PageNode | :red_circle: custom |
| 1 | AutonomousAccessResultNode | :red_circle: custom<br>:yellow_circle: premium |
| 1 | DataStoreDecisionNode | :red_circle: custom |
| 2 | ValidatedPasswordNode | :red_circle: custom |
| 2 | SelectIdPNode | :red_circle: custom |
| 1 | ValidatedUsernameNode | :red_circle: custom |
## Nodes (15)
| Display Name | Type | Classification | Id |
| ------------ | ---- | -------------- | ---|
| Social Login | InnerTreeEvaluatorNode | :red_circle: custom | 00b894da-4193-42cf-a544-1cbee31d06f8 |
| Count Login | IncrementLoginCountNode | :red_circle: custom | 04dd4568-48f4-4264-8539-2e1d119abc7e |
| Username? | ScriptedDecisionNode | :red_circle: custom | 13054b8b-bc63-4954-8e78-c7febb24711f |
| AA Login Risk | InnerTreeEvaluatorNode | :red_circle: custom | 1b6f03ae-d694-484c-8a24-a847104cb5cb |
| Login Page | PageNode | :red_circle: custom | 3d2b3d64-b8fc-416b-b8e0-e05f1502b49e |
| AA Record Failure | AutonomousAccessResultNode | :red_circle: custom<br>:yellow_circle: premium | 5e927eec-61d5-4ad0-83ea-8311fcf2c53f |
| U/P Login | DataStoreDecisionNode | :red_circle: custom | ca40167b-9a87-4937-9602-d453ea7cf6ef |
| Debug | ScriptedDecisionNode | :red_circle: custom | d985eba8-067f-4d62-925c-e9aa5046fad6 |
| Login Page | PageNode | :red_circle: custom | e41741ae-74bd-4838-84a2-50fdfbaa2637 |
| Progressive Profile | InnerTreeEvaluatorNode | :red_circle: custom | f750a7a8-cbc4-44b1-889d-b121e774e60d |
| Password | ValidatedPasswordNode | :red_circle: custom | ff55eaed-bea4-475d-a7dd-eb7d818fa80d |
| Select IDP | SelectIdPNode | :red_circle: custom | af614ad5-233d-4cbb-8f4e-462598b9658a |
| Username | ValidatedUsernameNode | :red_circle: custom | 2664240c-3a00-49f3-9c37-39ef391eca3c |
| Password | ValidatedPasswordNode | :red_circle: custom | f23a331a-966b-460e-aefa-2f033102f53a |
| Select IDP | SelectIdPNode | :red_circle: custom | 2d6be9fb-1dc8-4dd2-804c-0c5cfb8f5f28 |
## Scripts (2)
- 739bdc48-fd24-4c52-b353-88706d75558a AUTHENTICATION_TREE_DECISION_NODE - Check Username
- 3cb43516-ae69-433a-8787-501d45db14e9 AUTHENTICATION_TREE_DECISION_NODE - debug
