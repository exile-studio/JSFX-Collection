```txt
███████╗██╗  ██╗██╗██╗     ███████╗    ███████╗████████╗██╗   ██╗██████╗ ██╗ ██████╗
██╔════╝╚██╗██╔╝██║██║     ██╔════╝    ██╔════╝╚══██╔══╝██║   ██║██╔══██╗██║██╔═══██╗
█████╗   ╚███╔╝ ██║██║     █████╗      ███████╗   ██║   ██║   ██║██║  ██║██║██║   ██║
██╔══╝   ██╔██╗ ██║██║     ██╔══╝      ╚════██║   ██║   ██║   ██║██║  ██║██║██║   ██║
███████╗██╔╝ ██╗██║███████╗███████╗    ███████║   ██║   ╚██████╔╝██████╔╝██║╚██████╔╝
╚══════╝╚═╝  ╚═╝╚═╝╚══════╝╚══════╝    ╚══════╝   ╚═╝    ╚═════╝ ╚═════╝ ╚═╝ ╚═════╝

# Exile Studio – JSFX Collection

There are countless free and less-than-free plugins available; knew some, bought some, used some, but kept feeling on most of them there's something amiss.  
Might be quality-of-life-related UI controls, or just strictly **q u a l i t y   o f   s o u n d**, so I decided to take fate in my hands and code my own.  
After many late hours, scotch glasses, and ungodly curses, this is the result I wanted to share.

The philosophy can be summarized in the following key points:

---

### • EVERY non-linearity is implemented via ADAA  
(Anti-Derivative Anti-Aliasing — main reference: https://www.native-instruments.com/fileadmin/ni_media/downloads/pdf/VAFilterDesign_2.1.0.pdf)

Because in 2025 it is a crime against humanity not doing it, or making people pay 200 dollars just for the claim of it.  
In short: ADAA ensures non-linear stages (e.g., saturation) will not explode into an aliasing/intermodulation mess.  
It's not the definitive solution, but it's what can be handled (or better: what *I* can handle) via JSFX without growing suicidal.

---

### • UI controls reduced to the minimum without compromising flexibility  
Quick to understand, quick to set, quick to hear.  
Tune in, turn on, drop out.

---

### • Everyone has their own tastes and OCDs — these plugins are meant to only cover mine  
If they align with yours, good.  
If not, ¯\_(ツ)_/¯

---

# Included Plugins

### **Exile Stereo Delay LA**  
LA-style stereo delay and widener (LA as in Lord-Alge).  
- Tempo sync  
- Stereo offset: adds a +/- offset to left and right channels to add a widening effect (LA)
- HPF/LPF on repeats  
- ADAA tube-style saturation  

---

### **Exile 1176 Compressor**  
FET-style compression with proper attack/release ballistics.  
- Feed-forward GR detection  
- Classic ratios  
- ADAA-based FET saturation  

---

### **Exile SSL Bus Compressor**  
The bus glue compressor.  
- Smooth timing  
- Clean detection  
- Subtle color  
- ADAA saturation in the right spots  

---

### **Exile Gate**  
Smooth, musical gate inspired by real-world vocal/drum use.  
- Clean behaviour  
- Sidechain HPF  
- Adjustable hold  
- No zippering or clicks  

---

### **Exile Pultec EQ**  
A light, musical two-band EQ inspired by the classic curves.  
- Low boost + attenuation  
- High boost + attenuation  
- ADAA tube-style color after the filters  

---

### **Exile Pre**  
A subtle preamp-style saturator.  
- ADAA-based non-linearity  
- Integrated 2x oversampling  
- Volume-compensated internal sidechain (tunable LP frequency) for the saturated path.

---

### **Exile Auto Gain Staging**  
A simple gain-staging helper.  
- Learns peak level  
- Applies gain to hit chosen target  
- Two modes: learn (listen to the source audio to tune to the target volume) + apply
- Zero latency  

---

# Installation

1. Download the latest release ZIP.  
2. Open REAPER → `Options → Show REAPER resource path…`  
3. Drop the `.jsfx` files into the `Effects/` folder.  
4. Restart REAPER or rescan the FX list.  
5. Search for “Exile” in the FX browser.

---

# License

This project is released under **CC BY 4.0**.  
You may use, modify, or redistribute any of these plugins — including commercially —  
**as long as you provide attribution to “Michele Raggi - Exile Studio”.**

Full license:  
https://creativecommons.org/licenses/by/4.0/

---

# Disclaimer

All references to existing brands, products, hardware models, or company names  
are used purely for descriptive and comparative purposes.  
They are not endorsements, not affiliations, and definitely not official models.  
And yes — they’re written in clear text because, honestly, who the fuck cares.

---

# Support / Contact

None, but you can contact me at michele.raggi AT tuta.io  
No guarantees, no updates promised, no support system.  
Use at your own risk.
