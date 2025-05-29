# NoteAI
📚 App Summary
NoteAi is a note-taking application inspired by Notability, enhanced with AI-powered features. It supports handwritten and typed notes, synchronized audio recordings, and versatile document annotation. In addition, NoteAi introduces advanced AI features including live speech-to-text transcription, contextual summarization, semantic search, intelligent document answering to boost learning and productivity, and live note collaboration

#✏️ Core Features (Inspired by Notability)

Handwriting & Drawing
Apple Pencil compatibility
Tools: Pen, Highlighter, Eraser, Lasso, Shape Recognition
Typing Support
Mixed media notes (handwriting + text)
Audio Recording
Time-synced with notes
PDF & Document Annotation
Highlight, underline, write, and comment
Note Organization
Subjects, folders, tags, search

#🤖 AI Assistance Features

Live Transcription
Real-time conversion of speech into notes as users speak or during recordings.
Transcribed text appears in the note-taking area in sync with the audio timeline.
Useful for lectures, meetings, interviews, or brainstorming sessions.
AI Summarization & Contextual Notes
GPT-4 powered summarization of long transcriptions or typed content.
Generates bullet points, graphs/tables, and simplified explanations.
Context-aware note suggestions based on current topic and historical notes.
Smart Search
Instead of matching exact keywords, Smart Search understands the meaning of your question and surfaces results based on that.
Queries like “Show me all notes where the professor explained supply and demand.”, “Where are my calculus practice problems with integrals?” would return note snippets or a filtered list of notes
Document Q&A (Fill-in-the-Blank AI Answers)
AI scans user-uploaded documents (e.g. worksheets, question sets).
Identifies conceptual and computational questions.
Uses GPT to fill in blanks, solve math problems, and explain answers inline.
Ai Assistance (Optional)
Detects key terms, dates, equations, or concepts.
Highlights them in the document and adds tooltips or definitions.
Users can ask natural questions like “Summarize what i studied on July 4th” etc.
Helps in exam preparation and active learning.
Collaborative Note-Taking (Multi-User Live Sessions)
Multiple users can join a shared note session in real time.
Users can draw, type, and comment together.
Live cursors and user labels for visibility.
Ideal for classrooms, group studies, or team meetings.

#🚀 Tech Stack & Frameworks

#📱 Frontend (Cross-Platform)

React Native (iOS & Android)
Expo / Bare Workflow for Apple Pencil and native module access
Canvas Implementation:
iOS: Native module using Swift + PencilKit for high-performance Apple Pencil drawing
Android: Skia (react-native-skia) for high-performance canvas rendering
react-native-pdf for PDF annotation
redux / zustand for state management
react-navigation for screen flows

#🛠️ Backend
Node.js with Express.js for RESTful APIs
MongoDB (Mongoose) for note storage and user data
Firebase (for real-time syncing and auth alternative)
Socket.io for real-time transcription syncing
AWS S3 / Cloudinary for media storage (audio/PDFs)

🧠 AI Integrations
OpenAI Whisper / Google Speech-to-Text for transcription
GPT-4 (via OpenAI API) for summarization
LangChain / DeepEval for document analysis and interaction
Weaviate / Pinecone for semantic search with vector embeddings

#👨‍💼 Frontend Team Tasks

Implement Drawing Canvas:
Swift + PencilKit module for iOS
Skia canvas for Android fallback
Integrate PDF rendering and annotation with react-native-pdf
Build real-time transcription display overlay
UI for chat-based AI assistant within each note
Note organizer: folder creation, drag-drop, tags
Audio recording UI + waveform + timestamp linkage
Text editor with rich formatting and AI-suggested auto-fill

#📍 Backend Team Tasks

Setup user auth & session (JWT/Firebase Auth)
Design MongoDB schema for users, notes, audio, transcripts
Build API endpoints for notes CRUD, transcription, AI summary
Integrate Whisper/GPT APIs for transcription + summarization
Enable semantic vector search via Weaviate + OpenAI embeddings
Build PDF document parsing for question detection & AI fill-in
Real-time updates via WebSocket (Socket.io)

#🔗 Optional Stretch Goals

Cloud sync with Google Drive / iCloud using possible aws
Multi-language transcription + translation
AI voice assistant to control app hands-free


