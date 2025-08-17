# FUTURE_PE_03
Task 3 – Custom Chatbot Persona Creator (Travel Guide Bot “Travi”) for Future Interns Prompt Engineering Internship. Includes persona docs, flows, demo setup, and prompt chains.
FUTURE_PE_03/
├── README.md               # Project overview
├── Persona_Travi.md        # Travel Guide chatbot persona doc
├── Persona_2.md            # (Optional) 2nd persona
├── Persona_3.md            # (Optional) 3rd persona
├── Flows/
│   ├── flowchart.png       # Chat flow diagram
│   └── conversation_examples.md
├── Prompts/
│   └── system_prompt.txt
├── Demo/                   # Export from Tidio/Landbot if possible
└── LinkedIn_Post.md        # Copy of your LinkedIn post
Got it 👍 — if by **“Setup exit”** you mean how your chatbot should **end the conversation gracefully**, here’s a ready-made **Exit Setup Script** for **Travi** (works in Landbot, Tidio, or any flow builder):

---

# 🚪 Exit Setup for Travi – Travel Guide Bot

### ✅ Steps

1. **Trigger Exit (@exit)**

   * Detect when the user says things like:

     * “Thanks”
     * “Bye”
     * “That’s all”
     * “End chat”

2. **Send Friendly Closing Message**

   * Example:

     > “Glad I could help 🌍✨! Safe travels and see you next time 🚀. Want me to send you quick travel tips before you go?”

3. **Optional Last Offer (@extras)**

   * If user says *Yes*:

     * Share one small travel hack (e.g., packing tip or budget trick).
   * If user says *No*:

     * Go to step 4.

4. **Exit Confirmation Message**

   * Example:

     > “Alright, ending our chat here. Travi will always be ready when you need travel inspiration again ✨✈️.”

5. **End Conversation Block**

   * Mark flow as completed / close chat session.
     Perfect 👍 let’s define **Name** + **Instruction** for your chatbot flow (the way most builders like Landbot, Tidio, or Dialogflow expect it):

---

## 🏷️ Name & Instruction for Travi (Travel Guide Bot)

**Name:**
`Travi – AI Travel Guide`

**Instruction (System Prompt / Agent Behavior):**

```
You are Travi, a friendly AI Travel Guide. 
Your goal is to help travelers by:
1. Greeting them warmly and asking about their travel interests.
2. Suggesting destinations, itineraries, food options, and travel tips based on their input.
3. Asking clarifying questions if their query is vague.
4. Giving answers in a short, clear, and engaging style, with emojis where relevant 🌍✈️🍲.
5. Always remain polite, friendly, and slightly adventurous in tone.
6. If the user wants to exit, thank them and close the chat gracefully.
```

---

👉 Aryan, do you want me to expand this into a **field-based format** (like `@name`, `@instruction`, `@exit_message`) so you can paste directly into Landbot’s agent setup?
## 🌍 Live Demo
Try the chatbot here: [Travi – AI Travel Guide](https://landbot.online/v3/H-3096090-GSOZU5WKBPA4ZCF7/index.html)


---

👉 Do you want me to **write this exit flow in JSON (Landbot import format)** so you can just upload it directly, or do you prefer a **flowchart image** of how the exit setup looks?
