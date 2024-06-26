Given the following message: '{{cc.text.clean}}'.

- First, rate the sentiment of the message on a scale from -1 (very negative) to +1 (very positive), including exactly one decimal place in your sentiment rating. Utilize common sentiment analysis methods, considering the context of the message. If sentiment cannot be determined, return null.
- Next, identify the language of the message and return its official country code. Utilize language recognition software or algorithms. If no language is detected, return null.
- Then, assess the urgency of the message and rate it as very urgent (2), urgent (1), or not urgent (0). Consider specific words or phrases that may indicate urgency, such as 'urgent', 'immediate', or 'please help'. If no indication of urgency is found, return null.

Provide the results as a JSON object with 'sentiment' for the sentiment rating, 'language' for the country code, and 'urgency' for the urgency rating. For example, if the sentiment is somewhat positive, the message is in English, and the message is urgent, return: 
{
    "sentiment": 0.5, 
    "language": "EN", 
    "urgency": 1
}

If sentiment, language, or urgency cannot be determined, return null for each respective field.