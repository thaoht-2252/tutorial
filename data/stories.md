## greetings
* greet
  - utter_greet

## ask about contributing idea
* trigger_contribute_idea
  - utter_guide_idea

## contribute idea 
* trigger_contribute_idea
  - utter_guide_idea
* affirm
  - idea_form
  - form{"name": "idea_form"}
  - form{"name": null}
  - utter_confirm_idea_content
* affirm
  - utter_received_idea
  - action_reset_all_slots
* thankyou
  - utter_no_worries

## contributed idea but don't want to submit
* trigger_contribute_idea
  - utter_guide_idea
* affirm
  - idea_form
  - form{"name": "idea_form"}
  - form{"name": null}
  - utter_confirm_idea_content
* deny_submitting
  - utter_not_submit
  - action_reset_all_slots
* thankyou
  - utter_no_worries

## no idea path
* trigger_contribute_idea
  - utter_guide_idea
* deny
  - utter_goodbye

# thankyou
  - utter_no_worries

## say goodbye
* goodbye
  - utter_goodbye