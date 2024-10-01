# AI Image Metadata Editor
Single file pure HTML tool for viewing and editing AI image metadata locally on your web browser without the need of installation or internet connectivity. The tool is designed specifically for reading and editing PNG image metadata in the Automatic1111/Forge web UI format.

## Demo
https://xypher7.github.io/ai-image-metadata-editor

## Usage
No need for prior setup, just open the HTML file with the web browser of your choice and drag an image file. Alternatively, you can use the version hosted on GitHub through the link provided in the demo section.

### Adding Checkpoint Resources
Large files greater than 2GB rely on the 3rd party library <a name="unique-anchor-name" href='https://www.npmjs.com/package/hash-wasm'>hash-wasm</a> due to serverless HTML limitations. Online connectivity is required to fetch the dependency. Optionally, if you wish to maintain everything local, you may download the <a name="unique-anchor-name" href='https://cdn.jsdelivr.net/npm/hash-wasm@4/dist/sha256.umd.min.js'>sha256.umd.min.js</a> file, place it in the same directory as the HTML file, and replace this line
```html
<script src="https://cdn.jsdelivr.net/npm/hash-wasm@4/dist/sha256.umd.min.js"></script>
```
 with 
```html
 <script src="sha256.umd.min.js"></script>
```

## Features
- View and edit PNG metadata in Auto1111/Forge UI format.
- Drag and drop safetensors files to add resource to metadata.
- LoRA and Checkpoint resource links to CivitAI.
- Offline Execution. The tool is designed to be used offline and processing is entirely done on your browser.

![App Screenshot](https://image.civitai.com/xG1nkqKTMzGDvpLrqFT7WA/5b30fbe1-bbce-4e83-9b99-bcf11aa71ceb/original=true,quality=90/Screenshot%202024-09-29%20001102.jpeg)
