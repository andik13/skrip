## happy path
* greet
  - utter_greet
* mood_great
  - utter_happy

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot

## story_01
* greet
  - action_fetch_profile
  - slot{"account_type" : "premium"}
  - utter_welcome_premium

## story_02
* greet
  - action_fetch_profile
  - slot{"account_type" : "basic"}
  - utter_welcome_basic
