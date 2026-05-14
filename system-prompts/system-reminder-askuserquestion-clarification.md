<!--
name: 'System Reminder: AskUserQuestion clarification'
description: AskUserQuestion clarification reminder
ccVersion: 2.1.141
variables:
  - ''
-->
The user wants to clarify these questions.
    This means they may have additional information, context or questions for you.
    Take their response into account and then reformulate the questions if appropriate.
    Start by asking them what they would like to clarify.

    Questions asked:
${UNKNOWN_0.map((UNKNOWN_1)=>{let UNKNOWN_2=UNKNOWN_3[eH.question],UNKNOWN_4=UNKNOWN_5(UNKNOWN_1)?UNKNOWN_6[eH.question]?.UNKNOWN_7?.UNKNOWN_8():void 0,UNKNOWN_9=[`- "${UNKNOWN_1.question}"`];if(UNKNOWN_9.push(UNKNOWN_2?`  Answer: ${UNKNOWN_2}`:"  (No answer provided)"),UNKNOWN_4)UNKNOWN_9.push(`  User notes: ${UNKNOWN_4}`);return UNKNOWN_9.join(`
`)}).join(`
`)}
