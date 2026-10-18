# SoundCraft Web

Wersja webowa SoundCraft — profesjonalna stacja robocza audio (DAW) w przeglądarce.

- **URL:** [https://sound.lmk.one/](https://sound.lmk.one/)
- **Technologia:** Rust, WebAssembly, WebGPU / WebGL2, WebAudio, egui/eframe
- **Wydajność:** Kompilacja Fat LTO, pojedyncza jednostka generowania kodu (`codegen-units = 1`), pre-kompresja statyczna Gzip (`.wasm.gz`)
- **Funkcje:**
  - Akceleracja sprzętowa WebGPU z automatycznym przełączaniem na WebGL2
  - Ciemny interfejs (Dark Mode)
  - Polska wersja interfejsu (PL)
  - Obsługa parametru `?file=` (wczytywanie sesji i plików audio bezpośrednio z URL z fallbackiem CORS)
  - Wsparcie dla formatów: sesje `.scraftz`, pliki audio `.wav`, `.flac`, `.mp3`, `.ogg`, `.aiff`, `.caf`, `.m4a` oraz pliki `.mid` / `.midi`
