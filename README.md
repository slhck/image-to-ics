# Image to ICS

This is a simple website to convert an image to an ICS file.
The image can contain one or multiple events, and the output will be a single ICS file with all the events ready to be imported into your calendar.

## Usage

- Generate an API key in [OpenAI](https://platform.openai.com/api-keys)
- Enter your OpenAI API key in the field and click "Set OpenAI API Key"
  - The key will be stored in your browser's local storage, so it won't be sent to any other server.
  - You can remove it at any time
- Drop an image file on the page into the dropzone, or paste from the clipboard
- Optionally provide extra context for event parsing
- Click the "Convert" button
- Download the resulting ICS file

## Behind the scenes

The image is processed by an LLM to extract the events. The LLM used is gpt-4o-mini.
It is instructed to extract the events from the image and return them in an ICS format.

The whole code was <s>written</s> vibe-coded by Cursor with claude-3.5-sonnet initially, and other models later on.

## TODOs

- [ ] Add capability to upload images from URL
- [ ] Make it possible to just dump some unformatted text and have the LLM format it as an ICS file

## License

Copyright (c) Werner Robitza

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
