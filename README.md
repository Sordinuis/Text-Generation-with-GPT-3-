# Text-Generation-with-GPT-3-
Generate text using OpenAI's GPT-3 language model (requires API access).
import openai

openai.api_key = 'your-api-key'
prompt = "Once upon a time in a land far, far away..."

response = openai.Completion.create(
    engine="text-davinci-003",
    prompt=prompt,
    max_tokens=100
)

generated_text = response['choices'][0]['text']
print(generated_text)
