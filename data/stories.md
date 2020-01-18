## happy path
* greet
  - utter_greet
* mood_great
  - utter_happy

 ## finduse affirm path
* greet
 - utter_greet
* uses{"device":"oximeter"}
 - utter_usage
 - utter_did_that_help
* affirm
 - utter_happy
* thanks
 - utter_goodbye

 ## finduse deny path
* greet
 - utter_greet
* uses{"device":"oximeter"}
 - utter_usage
 - utter_did_that_help
* deny
 - utter_please

## findwork path
* working
  - utter_working

 ## battery path
* battery{"battery_life":"low battery"}
  - utter_battery
<!-- 
## findbutton path
* button{"device":"oximeter"}
 - utter_button  -->

## display path
* display
  - utter_display


## setup path
* setup
  - utter_setup

<!-- ## findreading path
* reading{"normal_reading":"default readings"}
 - utter_normalreading
* reading{"abnormal_reading":"below normal"}
 - utter_abnormalreading} -->

## findcorrectness path
* correctness
  - utter_correctness

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
