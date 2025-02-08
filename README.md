flowchart TD
    A[User Signs ASL Gesture] -->|Camera Captures Frame| B(Preprocessing)
    B -->|Feature Extraction| C(Deep Learning Model)
    C -->|ASL Gesture Classification| D{Gesture Matches Vocabulary?}
    D -- Yes --> E[Convert to Text Output]
    E -->|Optional TTS| F[Audio Output]
    D -- No --> G[Request User to Repeat Gesture]
