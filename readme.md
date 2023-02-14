Inspired by a video of Dan Vega I followed along his video and create this cli to talk to ChatGPT

Get your own key at: https://platform.openai.com/account/api-keys

See documentation: https://platform.openai.com/docs/api-reference/completions

This code makes this request possible:

POST https://api.openai.com/v1/completions
Content-Type: application/json

Authorization: Bearer YOUR_KEY_HERE

{
"model": "text-davinci-001",
"prompt": "How many kilometers are in a mile?",
"temperature": 1,
"max_tokens": 100
}

The result should contain something like:  "text": "\n\n1 mile = 1.609 kilometers"
