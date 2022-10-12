# AA-Login
Autonomous Access Login
## Status
:white_check_mark: enabled
## Classification
:purple_circle: cloud, :yellow_circle: premium
## Categories/Tags
Authentication, Social Authentication, Adaptive, Autonomous Access
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
- 3 InnerTreeEvaluatorNode (:green_circle: standard)
- 1 IncrementLoginCountNode (:green_circle: standard)
- 2 ScriptedDecisionNode (:green_circle: standard)
- 2 PageNode (:green_circle: standard)
- 1 AutonomousAccessResultNode (:purple_circle: cloud, :yellow_circle: premium)
- 1 DataStoreDecisionNode (:green_circle: standard)
- 2 ValidatedPasswordNode (:green_circle: standard)
- 2 SelectIdPNode (:green_circle: standard)
- 1 ValidatedUsernameNode (:green_circle: standard)
## Nodes (15)- 00b894da-4193-42cf-a544-1cbee31d06f8 (:green_circle: standard) InnerTreeEvaluatorNode - Social Login
- 04dd4568-48f4-4264-8539-2e1d119abc7e (:green_circle: standard) IncrementLoginCountNode - Count Login
- 13054b8b-bc63-4954-8e78-c7febb24711f (:green_circle: standard) ScriptedDecisionNode - Username?
- 1b6f03ae-d694-484c-8a24-a847104cb5cb (:green_circle: standard) InnerTreeEvaluatorNode - AA Login Risk
- 3d2b3d64-b8fc-416b-b8e0-e05f1502b49e (:green_circle: standard) PageNode - Login Page
- 5e927eec-61d5-4ad0-83ea-8311fcf2c53f (:purple_circle: cloud, :yellow_circle: premium) AutonomousAccessResultNode - AA Record Failure
- ca40167b-9a87-4937-9602-d453ea7cf6ef (:green_circle: standard) DataStoreDecisionNode - U/P Login
- d985eba8-067f-4d62-925c-e9aa5046fad6 (:green_circle: standard) ScriptedDecisionNode - Debug
- e41741ae-74bd-4838-84a2-50fdfbaa2637 (:green_circle: standard) PageNode - Login Page
- f750a7a8-cbc4-44b1-889d-b121e774e60d (:green_circle: standard) InnerTreeEvaluatorNode - Progressive Profile
- ff55eaed-bea4-475d-a7dd-eb7d818fa80d (:green_circle: standard) ValidatedPasswordNode - Password
- af614ad5-233d-4cbb-8f4e-462598b9658a (:green_circle: standard) SelectIdPNode - Select IDP
- 2664240c-3a00-49f3-9c37-39ef391eca3c (:green_circle: standard) ValidatedUsernameNode - Username
- f23a331a-966b-460e-aefa-2f033102f53a (:green_circle: standard) ValidatedPasswordNode - Password
- 2d6be9fb-1dc8-4dd2-804c-0c5cfb8f5f28 (:green_circle: standard) SelectIdPNode - Select IDP
## Scripts (2)
- 739bdc48-fd24-4c52-b353-88706d75558a AUTHENTICATION_TREE_DECISION_NODE - Check Username
- 3cb43516-ae69-433a-8787-501d45db14e9 AUTHENTICATION_TREE_DECISION_NODE - debug
