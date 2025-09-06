# Interactive Installation Program

This repository contains the frontend program developed for an interactive artwork presented at the exhibition **「尾角典子 #拡散」"Noriko Okaku: #spread"** held at [十和田市現代美術館 Towada Art Center](https://towadaartcenter.com/exhibitions/okaku_noriko/) (Satellite venue: *space*, July 6 – September 8, 2024).

The backend system processes the audience’s spoken input (their name) and generates text, images, and music in real time as part of the installation experience.

### Processing Flow
1. **Name Capture**  
   Receives voice input from the microphone and extracts the spoken name.  

2. **Text Construction**  
   Incorporates the name into a dynamically created sentence using a **custom algorithm** (not AI-generated).  

3. **Image Generation**  
   Sends the constructed text as a prompt to the **DALL·E 3 API**, producing a unique image.  

4. **Music Generation**  
   Uses the same text as a prompt for the **Suno AI API**, generating original music.  

This pipeline integrates language, vision, and sound to create a multi-sensory, audience-driven artwork.

## Role and Contribution
I was responsible for the **overall programming of the artwork**, including both frontend and backend systems.  
This repository documents the **backend system**, which specifically:

- Provides the algorithm to embed the audience’s name into text.
- Implements API calls to external generative services (OpenAI DALL·E 3, Suno AI).
- Handles synchronization between generated text, images, and music.
- Exchanges data seamlessly with the [frontend repository](https://github.com/NMinato77/okaku-whole-front).

## Technical Notes
- **Language**: Python  
- **APIs Used**:  
  - OpenAI (DALL·E 3 for image generation)  
  - Suno AI (for music generation)  
- **Functionality**: Input processing, text construction, external API orchestration  

This repository documents the backend logic.  
The frontend system (e.g., display synchronization and input handling) is maintained separately.

---

## Exhibition Details
- **Title**: 尾角典子 #拡散 *Noriko Okaku: #spread*  
- **Dates**: July 6 – September 8, 2024  
- **Venue**: 十和田市現代美術館 Towada Art Center (Satellite venue *space*)  
- **Link**: [towadaartcenter.com/exhibitions/okaku_noriko](https://towadaartcenter.com/exhibitions/okaku_noriko/)

---

## Acknowledgments
This project was realized as part of the exhibition ** 「尾角典子 #拡散」"Noriko Okaku: #spread"** at 十和田市現代美術館 Towada Art Center (July 6 – September 8, 2024).  
I would like to thank artist **Noriko Okaku** for her creative vision and collaboration,  
Chieko Nakagawa for her kind support,  
Fu Sakai for inviting me to this project,  
and the **Towada Art Center** for providing the platform and support to present this work.

---

## License
This code is released under the MIT License.  
Please see the [LICENSE](./LICENSE) file for details.
