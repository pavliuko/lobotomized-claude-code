<!--
name: 'System Reminder: AskUserQuestion clarification'
description: AskUserQuestion clarification reminder
ccVersion: 2.1.141
variables:
  - QUESTIONS
  - ANSWERS_BY_QUESTION
  - HAS_TEXT_INPUT_NOTES
  - QUESTION_STATES
-->
The user wants to clarify these questions.
    This means they may have additional information, context or questions for you.
    Take their response into account and then reformulate the questions if appropriate.
    Start by asking them what they would like to clarify.

    Questions asked:
${QUESTIONS.map((QUESTION)=>{let ANSWER=ANSWERS_BY_QUESTION[QUESTION.question],USER_NOTES=HAS_TEXT_INPUT_NOTES(QUESTION)?QUESTION_STATES[QUESTION.question]?.textInputValue?.trim():void 0,LINES=[`- "${QUESTION.question}"`];if(LINES.push(ANSWER?`  Answer: ${ANSWER}`:"  (No answer provided)"),USER_NOTES)LINES.push(`  User notes: ${USER_NOTES}`);return LINES.join("\n")}).join("\n")}
