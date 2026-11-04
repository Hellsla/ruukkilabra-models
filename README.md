# Ruukkilabra models

Large model files for the read-aloud voice of Ruukkilabra (https://hellsla.github.io/fysiikkalabra/site/),
kept out of the main site repository. Served with GitHub Pages at https://hellsla.github.io/ruukkilabra-models/
(the same origin as the site). `readaloud.js` loads them from there (constant `MODEL_BASE`) only after the student
chooses the better voice in the Voice menu.

| Folder | Contents | Licence |
|---|---|---|
| `supertonic3-v1/` | Supertonic 3 by Supertone Inc. (sherpa-onnx conversion, see its README), ~145 MB | BigScience OpenRAIL-M, https://huggingface.co/Supertone/supertonic-3/blob/main/LICENSE |
| `ort/` | onnxruntime-web 1.22.0 (Microsoft): ort.webgpu.min.js + WebAssembly runtime, ~22 MB | MIT, https://github.com/microsoft/onnxruntime |

The OpenRAIL-M use restrictions apply to everyone who uses the voice; Ruukkilabra uses it only to read its own
learning materials aloud. A changed model goes in a new versioned folder (`supertonic3-v2/`), so cached copies in
browsers never mix two models.
