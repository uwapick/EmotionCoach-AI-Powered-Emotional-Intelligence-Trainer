# EmotionCoach-AI-Powered-Emotional-Intelligence-Trainer
EmotionCoach uses emotion recognition and ML to analyze users' emotional responses in various situations and provides personalized coaching to help develop emotional intelligence skills.
import random

def recognize_emotion(user_input):
    """Simulate emotion recognition based on user input."""
    emotions = ['happy', 'sad', 'angry', 'anxious', 'excited', 'disappointed']
    # In a real app, analyze the user_input to determine the emotion
    return random.choice(emotions)

def provide_coaching(emotion):
    """Provide personalized coaching based on the recognized emotion."""
    coaching_advice = {
        'happy': "It's great to see you happy! Remember, spreading happiness can be contagious.",
        'sad': "It's okay to feel sad. Try to understand what's making you sad and express your feelings.",
        'angry': "Anger can be challenging. Take deep breaths and try to express your feelings calmly.",
        'anxious': "Anxiety can be tough. Focus on what you can control and take things one step at a time.",
        'excited': "Excitement is wonderful! Channel this energy into productive activities.",
        'disappointed': "Disappointment is part of life. Reflect on what happened and how you can move forward."
    }
    return coaching_advice.get(emotion, "It's interesting to feel that way. Let's explore this emotion together.")

def main():
    print("Welcome to EmotionCoach, your AI-powered emotional intelligence trainer.")
    user_input = input("How are you feeling today? Describe your feelings or the situation: ")
    recognized_emotion = recognize_emotion(user_input)
    print(f"Based on your input, it seems you're feeling {recognized_emotion}.")
    coaching = provide_coaching(recognized_emotion)
    print(coaching)

if __name__ == "__main__":
    main()
