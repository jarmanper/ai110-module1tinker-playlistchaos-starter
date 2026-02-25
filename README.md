# Summary

The core challenge of this activity is learning to treat AI-generated code as a hypothesis, not pure truth, even when it looks polished and runs without errors. The Playlist Chaos app demonstrates how subtle logic errors can hide in plain sight! One example is a song search that claims to work but returns wrong results, classification rules that contradict themselves, and statistics that don't add up. Students must develop a debugging workflow that combines three skills. First is observing unexpected behavior in the UI (the "what"), tracing that behavior back to specific code (the "where"), and using AI as a thinking partner to understand root causes rather than just getting quick fixes (the “why”/”how”).

## Where students struggle most

Where students will struggle most: Two patterns emerge pretty visibily. First, students often skip the exploration phase and jump straight to code, which means it is likely that they miss the crucial insight that using the app is debugging. Second, when Copilot offers an explanation, students accept it without comparing it to what they actually saw. The AI might explain what the code should do, but miss what it actually does. For example, a search function might look case-insensitive in the logic, but if the input isn't normalized first, it will fail. Copilot can explain both interpretations, and it’s the student's job to decide which one matches reality.

## Where AI helped vs. misled

Where AI helped vs. misled: Copilot excels at explaining what a block of code does line-by-line, ask it to walk through the logic and it's highly reliable. It struggles with detecting the gap between intent and implementation. It will confidently explain a function's purpose without noticing that the function never actually enforces it. The most useful Copilot questions aren't "what does this do?" but "what assumptions does this code make, and what happens if they're violated?" and "why would this behavior surprise a user?"

## Guidance without answers

Guidance without answers: When a student shows me a bug they found, I will resist the urge to point them at the fix immediately. Instead, I’ll ask - "What did the app do? What did you expect instead? Now find the function that controls that behavior. Can you walk me through what that code does step-by-step?" It's important to make them build the connection between observation and code themselves, because that's where the real learning lies. I'll Let them use Copilot to understand, but make them decide whether Copilot's explanation actually matches their observations.
