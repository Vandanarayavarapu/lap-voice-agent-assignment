# Home Credit LAP Voice Agent: Test Call Transcripts

Platform: Retell AI (Single Prompt Agent). Agent: Priya (female). Customer: Vandana. Language: English.
Note: some customer words look odd (e.g. "new load", "one cup") because of speech-to-text errors in the transcript; the agent handled them by confirming.

---

## Call 1: Eligible customer (full qualification and handoff)
Expected: all 7 items collected, then handoff to senior loan expert.
Result: PASS

agent: Hello, am I speaking with Vandana?
user: Yes. Speaking.
agent: I'm Priya from Home Credit. Is this a convenient time for a quick call about a special offer for
user: Yes. Go
agent: existing customers?
user: ahead.
agent: As a valued Home Credit customer, you may be eligible for a pre-approved Loan Against Property of up to seventy-five lakh rupees. Would you be looking for a fresh loan, or is there already a loan on the property?
user: It's a new low.
agent: For a fresh loan, is the property residential, commercial, or industrial?
user: It's a residential house, and then the only one.
agent: Is the house solely owned by you, or jointly owned with someone else?
user: I have the original purpose.
agent: Do you have the original property documents available for verification?
user: I have.
agent: What loan amount would you like to apply for?
user: I needed around fifty lakhs.
agent: And are you salaried or self-employed?
user: I'm salaried, and my salary comes to my bank account.
agent: What's the approximate current market value of the house?
user: Worth around one cup.
agent: Could you confirm the property's approximate value in rupees?
user: Yes.
agent: Did you mean the property is worth around one crore rupees?
user: Yes.
agent: What loan tenure would you prefer, between three and fifteen years?
user: Ten years.
agent: Thank you. A senior loan expert will call shortly to discuss the next steps and exact interest rate. Thank you for your time.
user: Okay. Thank you.
agent: You're welcome. Have a good day.

---

## Call 2: Agricultural property (immediate disqualification)
Expected: polite rejection, call ends, no further questions.
Result: PASS

agent: Hello, am I speaking with Vandana?
user: Yes. Speaking.
agent: I'm Priya from Home Credit. As a valued customer, you may be eligible for a pre-approved Loan Against Property of up to seventy-five lakh rupees. May I ask a few quick questions to see if it suits you?
user: Yes. Go ahead.
agent: Are you looking for a fresh loan, or is there already a loan on the property?
user: The new load.
agent: For the fresh loan, is the property residential, commercial, or industrial?
user: (unintelligible audio)
agent: Can you repeat the property type: residential, commercial, or industrial?
user: Agricultural land.
agent: I'm sorry, agricultural property doesn't meet the criteria for this specific offer at this time. Thank you for your time.

---

## Call 3: Cash income (immediate disqualification)
Expected: polite rejection, call ends.
Result: PASS

agent: Hello, am I speaking with Vandana?
user: Yes. Speaking.
agent: I'm Priya from Home Credit. As a valued customer, you may be eligible for a pre-approved Loan Against Property of up to seventy-five lakh rupees. May I ask a few quick questions to see if it suits you?
user: Yes. Go ahead.
agent: Would this be a fresh loan, or is there already a loan on the property?
user: New loan.
agent: What type of property is it: residential, commercial, or industrial?
user: It's a commercial shop, and I'm the only owner.
agent: Do you have the original property documents available for verification?
user: Yes. I have the original documents.
agent: How much loan amount are you looking for?
user: I need around thirty lines.
agent: Could you confirm the amount in rupees?
user: Around thirty legs.
agent: Do you mean around thirty lakh rupees?
user: Yeah.
agent: What do you do for work: salaried or self-employed?
user: I run my own business, and my income isn't cash.
agent: Is your income mainly received in your bank account?
user: No. I run my own business. And my income is in cash.
agent: I'm sorry, but this specific offer requires income to be received through a bank account, so you don't meet the criteria at this time. Thank you for your time.

---

## Call 4: Existing loan / EMI reduction (transfer logic)
Expected: loan-transfer specialist message, call ends, no eligibility questions.
Result: PASS

agent: Hello, am I speaking with Vandana?
user: Yes. Speaking.
agent: I'm Priya from Home Credit. As a valued customer, you may be eligible for a pre-approved Loan Against Property of up to seventy-five lakh rupees. May I ask a few quick questions to see if it suits you?
user: Go ahead.
agent: Will this be a fresh loan, or is there already a loan on the property?
user: I already have a loan on this property. I want to reduce my EMI.
agent: Thank you for sharing that. Since there's already a loan on the property and you'd like to reduce your EMI, our loan-transfer specialist will contact you shortly to help. Thank you for your time.

---

## Call 5: Busy customer (callback)
Expected: no pitch, callback time captured, call ends.
Result: PASS

agent: Hello, am I speaking with Vandana?
user: Yes. Speaking.
agent: I'm Priya from Home Credit. Is this a convenient time to speak briefly about a special offer for existing customers?
user: I'm busy right now. I'm in a meeting. Call me tomorrow at five PM.
agent: Alright, I'll arrange a callback tomorrow at five PM. Thank you for your time.

---

## Call 6: Loan above 75 lakh, customer declines the maximum
Expected: agent explains the 75 lakh limit and asks to proceed with 75 lakh; ends politely on "no".
Result: PASS

agent: Hello, am I speaking with Vandana?
user: Yes. Speaking.
agent: I'm Priya from Home Credit. As a valued customer, you may be eligible for a pre-approved Loan Against Property of up to seventy-five lakh rupees. May I ask a few quick questions to see if it suits you?
user: Go ahead.
agent: Would this be a fresh loan, or is there already a loan on the property?
user: It's a new logo.
agent: Just to confirm, do you mean it's a fresh loan on the property?
user: A new loan.
agent: What type of property is it: residential, commercial, or industrial?
user: It's a residential house. I'm the only owner.
agent: Do you have the original property documents available for verification?
user: Yes. I have the virtual campus.
agent: Just to confirm, do you have the original property documents available for verification?
user: Yes. I have.
agent: How much would you like to borrow?
user: I did ninety lakhs.
agent: The offer is available up to seventy-five lakh rupees. Would you like to proceed with seventy-five lakh?
user: No.
agent: Thank you for your time. Since the offer is available up to seventy-five lakh rupees, we won't proceed further.

---

## Call 7: Loan above 75 lakh, customer accepts the maximum
Expected: agent continues the checklist with 75 lakh, then hands off after all 7 items.
Result: PASS

agent: Hello, am I speaking with Vandana?
user: Yes. Speaking.
agent: Hi Vandana, I'm Priya from Home Credit. Is this a convenient time for a quick call?
user: Yes. Go ahead.
agent: As a valued Home Credit customer, you may be eligible for a pre-approved Loan Against Property of up to seventy-five lakh rupees. Would you be looking for a fresh loan, or is there already a loan on the property?
user: It's a fresh loan.
agent: What type of property is it: residential, commercial, or industrial?
user: A residential house, and I'm the only owner.
agent: Is the original property document available for verification?
user: Yes. I have the personal papers.
agent: What loan amount would you like to apply for?
user: I need ninety lakhs.
agent: The offer is available up to seventy-five lakh rupees. Would you like to proceed with seventy-five lakh?
user: Seventy five lakhs is fine.
agent: What do you do for work, and is your income received in your bank account?
user: Salaried, and my salary comes to my bank account.
agent: What's the approximate current market value of the property?
user: The house is what? Around one crore.
agent: And how many years of tenure would you prefer for the loan?
user: Years.
agent: How many years would you prefer for the loan tenure?
user: Twelve years.
agent: Thank you, Vandana. A senior loan expert will call you shortly to discuss the next steps and exact interest rate.

---

## Call 8: Interest-rate diversion and out-of-order answers
Expected: agent does not invent a rate, captures out-of-order facts (house + joint ownership), does not re-ask them, continues with next missing item.
Result: PASS

agent: Hello, am I speaking with Vandana?
user: Yes. Speaking.
agent: I'm Priya from Home Credit. Is this a convenient time to speak briefly?
user: Yes. Go ahead.
agent: As a valued Home Credit customer, you may have a pre-approved Loan Against Property offer up to seventy-five lakh rupees. Would you like me to check if it suits you?
user: A new load.
agent: Do you mean a new, fresh loan against your property?
user: Yes.
agent: What type of property is it: residential, commercial, or industrial?
user: A restaurant? House. Jointly honored with my brother, What is the interest rate?
agent: A house is residential, and joint ownership is fine. The exact interest rate will be shared by the senior loan expert; do you have the original property documents available for verification?
user: Yes. I have
agent: What loan amount would you like?
user: Forty lakhs.
agent: What do you do for work?
user: I'm salaried, and it comes to my bank.
agent: What's the approximate current market value of the property?
user: Around eighty lakhs.
agent: How long would you like the loan tenure to be, between three and fifteen years?
user: Fifty fifteen years.
agent: Did you mean fifteen years for the loan tenure?
user: Yes.
agent: Thank you. Based on the details you shared, a senior loan expert will call you shortly to discuss the next steps and exact interest rate.
