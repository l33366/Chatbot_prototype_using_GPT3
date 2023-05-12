# Chatbot_prototype_using_GPT3
Here a chatbot is devoloped using gpt3, The repo includes the jasonl file that consists the format on which the data was fed in
install openai
while True:
  prompt1=input("ME: ")
  openai.api_key = ("Enter your own OpenAI API")
  response = openai.Completion.create(
    model="curie:ft-personal-2023-03-17-11-35-41",
    prompt=prompt1,
    temperature=0.7,
    max_tokens=15,
    top_p=1,
    frequency_penalty=0,
    presence_penalty=0
    )
  print("BOT: ",response['choices'][0]['text'])
