# Sound Science: Audifying the Sun

*Robert L. Alexander. IEEE Computer Graphics and Applications, vol. 46, no. 4, pp. 143-150, July/Aug. 2026. DOI 10.1109/MCG.2026.3694282. Author's copy. Markdown converted from the published PDF on 2026-09-10 with column-aware extraction; use for lookups, the PDF is the source of truth.*

EDITORS: Bruce D. Campbell, bcampbel01@risd.edu Francesca Samsel, fsamsel@tacc.utexas.edu On 5 September 2022, a car-sized spacecraft made of carbon composite and titanium was screaming through the void at over half a million miles per hour. It had been falling sunward for four years, with each Venus flyby tightening the orbit. The Parker 0272-1716 © 2026 IEEE. All rights reserved, including rights for text and data mining, and training of artificial intelligence and similar technologies. DOI: 10.1109/MCG.2026.3694282 This is the author's version of the article published in IEEE Computer Graphics and Applications, vol. 46, no. 4, pp. 143– 150, July/Aug. 2026.

Solar Probe (PSP) had already done what no spacecraft had done before: punched through the Sun’s outer atmosphere and survived. It was the fastest human-made object in existence, and the closest thing we had ever sent to a star. And the star was waking up.

Back at Johns Hopkins Applied Physics Lab (APL) in Maryland, project scientist Nour Raouafi knew this encounter would be different. Solar Cycle 25 was roaring ahead of every prediction. Earth-sized sunspots were blooming across the surface. “Nobody has ever flown through a solar event so close to the Sun before,”

*FIGURE 1. The moment of impact as the Wide-field Imager for Solar Probe (WISPR) camera captures a CME sweeping past PSP at 14 solar radii. Color reveals the motion of the solar wind plasma between video frames [NASA/Naval Research Laboratory (NRL)/Johns Hopkins University Applied Physics Laboratory (JHUAPL)].*

DEPARTMENT: ART ON GRAPHICS Sound Science: Audifying the Sun Robert L. Alexander , Space Science Institute, Boulder, CO, 80301, USA and also Arthur C. Clarke Center for Human Imagination, University of California San Diego, La Jolla, CA, 92093, USA Audification transforms data directly into sound, enabling the human auditory system to detect patterns that visual analysis overlooks. This article traces two decades of applying audification to NASA heliophysics data: from discovering a better thermometer for the Sun's corona by listening to the solar wind, to controlled studies where trained ears caught four times more anomalies than trained eyes, to projects where thousands of volunteer listeners discovered things no one expected. The silent age of space exploration is ending.

IEEE Computer Graphics and Applications. 1 he said in a NASA science editorial, “The data would be totally new.” He was right.

PSP was approximately 14 solar radii (5.6 million miles) from the surface of the Sun when sunspot region AR3088 exploded. Billions of tons of superheated plasma launched into space at 840 mi/s with a shockwave racing ahead of the mass. Had the eruption been aimed at Earth, it would have rivaled the most powerful solar storm in recorded history, the kind that blacks out entire continents. But it wasn't aimed at Earth. It was aimed at Parker.

The Wide-field Imager for Solar Probe (WISPR) camera saw it coming first: a wall of light sweeping across the field of view (see Figure 1). Then the shock front hit. Behind PSP’s 4.5-in carbon heat shield, designed to withstand 2,500°F, the SWEAP instruments were suddenly inside a monster coronal mass ejection (CME). Particle density surged as the shock front tore past the spacecraft, and PSP captured the whole event in glorious detail. “You try simplified models to explain certain aspects of the event,” said Orlando Romeo, the UC Berkeley physicist who published the event in the Astrophysical Journal,1 “but when you are this close to the Sun, none of these models can explain everything.”

I agree with Romeo, models can’t tell the entire story. PSP downloaded a treasure trove of data from this event, but traditional approaches to making sense of it bring us no closer to the experience of superheated helium ions colliding with a Faraday cup at 3 million mi/h. To get closer, to step inside the CME, we need one of the most sensitive instruments for frequency analysis on the planet. As luck would have it, you were born with two of them.

The human auditory system is capable of parsing multiple simultaneous streams of information, detecting frequency shifts of less than 1%, and resolving temporal detail at a rate 100 times finer than vision. Audification transforms data samples directly into audio samples, such that a million data points may be perceived in just seconds. No information is lost, and frequencies in the data emerge as frequencies in the resulting sound. When the APL team released their video of this encounter on YouTube, the sound in the background was magnetic field data that I had converted to sound. Nearly 800 million magnetometer samples across three components of the magnetic field, spatialized and temporally compressed into 40 s of audio. As a data audification specialist, this is my work: taking complex and multivariate datasets and bringing them to life through sound.

## AUDIFYING A CME

So what does a CME sound like? The dynamic range of the CME spans 70 dB, the difference between a whisper and a jackhammer, and the shock imparted enough intensity to clip the instrument itself. The magnetic field never settles, the baseline magnitude of each component drifts, producing what audio engineers call a direct current offset (DC offset). In short, loaded into Logic Pro, these audio files are a mixing engineer’s worst nightmare.

When translating the solar magnetic field into sound, magnetometers become your microphones. PSP’s fluxgate magnetometer captures multiple directional components of the magnetic field, and each can be used to add dimensionality to the final mix. The tangential and normal components contain the action. Panned hard left and right, they create a wide stereo image that jumps out of the speakers.

Each component contains over 260 million samples stretching nearly three and a half hours in length, and the WISPR video they need to match is 40 s long. Two complementary approaches make this possible. The first resamples the original data directly, preserving transient detail but pitch-shifting the signal more than eight octaves upward. The solar wind is fractal in nature, so the pitch shift reveals layers of structure at different timescales, but the low-frequency rumble is lost. A parallel layer breaks the signal into its frequency components, compresses the timeline, and rebuilds the sound at the original pitch. Layered together, the two approaches reconstruct a broadband spectrum: the complete sound of the solar magnetic field. The core resampling algorithm is now integrated into NASA’s Coordinated Data Analysis Web, where any time series in the heliophysics archive, from any mission, is available as audio.

The mastering chain shapes the full dynamic range of the star into something the human ear can hold: filtering the DC offset, suppressing harsh resonances, and balancing low-end weight against transient punch, while remaining true to the source data.

This is just the magnetic field. Working with wave physicist David Malaspina at the University of Colorado, we added high-frequency electric field data captured at 150,000 samples per second. At their native speed, these waves are ultrasonic. We slowed them down, time-aligned them to the WISPR visuals, and stretched the moment of impact like bullet time in The Matrix. The magnetic field rushes past 22,000 times faster than real time while the electric field unfolds seven times slower, a 150,000-fold difference.

Suddenly the CME wasn’t just a rumble. It was roaring, with high-frequency waves swirling around the shock front like wind tearing through a canyon. Two evolving spectral peaks in the electric field data, centered around 360 and 580 Hz, fall within the range of human vocal formants. The roaring quality of the audio is not a metaphor. The final version was released through the NASA Heliophysics Digital Resource Library in January 2025.2 This was the latest in a century-long tradition of listening to the cosmos.

## EARS TO THE STARS

*FIGURE 2. Descending whistler-mode waves observed by the Van Allen Probes.*

If you've seen the movie Contact, you know the scene: Jodie Foster, headphones on at the Very Large Array, listening to radio signals from space. The film is fiction, but the science is very real. In 1919, Barkhausen heard "a very remarkable whistling note" in a telephone receiver: radio emissions from lightning, sweeping downward as they dispersed through the magnetosphere (see Figure 2).

Over a decade later, Karl Jansky built a rotating antenna on a Model T chassis, pointed it at the sky, and heard something no one could explain: a faint steady static that peaked every 23 h and 56 min, cycling not with the Sun but with the stars. He was listening to cosmic radio emissions from the center of the Milky Way, and radio astronomy was born.

The discoveries kept coming. Electromagnetic bursts at dawn sounded so much like birdsong that researchers called them dawn chorus. Trapped plasma waves rattling inside the magnetosphere became simply “hiss.” When narrow-band electromagnetic noise at roughly 100 Hz was played through a speaker, it didn’t need a technical name. It sounded like a thundering roar on the Serengeti, and space physicists to this day are still unraveling the secrets of “lion roars.”

The vocabulary of space physics has auditory roots, and discoveries made through listening stretch back over a century. In 1982, when Voyager 2 flew past Saturn and returned a stream of data full of anomalous noise bursts, visual analysis came up empty. So the team listened, and the sound was unmistakable: a hailstorm. Bits of Saturn’s rings were pelting the spacecraft. Yet another discovery began with listening, but the method never took hold. No one had formalized audification as a tool that could stand alongside visualization in the research process.6

## THE CHALLENGE

“Show me something new with our data.” Thomas Zurbuchen was an intimidating figure. He went on to become the head of all science at NASA, and in that moment he was my Ph.D. advisor at the University of Michigan. Sitting in his office at the Space Research Building, the subtext was abundantly clear. NASA was pulling back on Education and Public Outreach. I was running out of runway, and needed to produce a result.

Thomas had bet on an idea: that we could hear something in his team’s satellite data that they couldn’t see. Solar wind measurements are turbulent, full of overlapping signals, and that’s exactly where trained ears might have an advantage. I’d been composing and producing music my whole life, and had recently begun exploring generative systems that translated the movement of dancers into sound in real time. Mary Simoni, Chair of the Performing Arts Technology department, had taken me under her wing and saw the connection before anyone else did. She introduced me to the Solar and Heliospheric Research Group, the team July/August 2026 IEEE Computer Graphics and Applications. 3 behind NASA’s Solar Wind Ion Composition Spectrometer (SWICS) aboard the ACE satellite.

SWICS captures helium ion velocities, elemental abundances, and charge state ratios as the solar wind streams past at hundreds of miles per second. They were tracking particles colliding with a sensor. I was tracking bodies colliding on a stage. For this research, I unplugged the dancers and plugged in the Sun.

My initial idea was to map data to musical parameters, an approach known as parameter mapping sonification. The velocity of the solar wind, I found, can control the cutoff frequency of a bandpass filter placed over pink noise, producing a sweeping wind sound that rises and falls with the solar wind itself. The result sounds like terrestrial wind swirling through the trees, intuitive and immediately understood.

With one intuitive mapping in my pocket, I went looking for more. Carbon exists in the solar wind at different ionization levels, and these charge states act as a thermometer for the corona. I recorded the voice of my sister, Amanda Alexander, and mapped six carbon charge states onto six vocal layers. When one charge state goes up, another comes down, and the prevalence of each modulates the volume of its corresponding layer. Higher ionization states bring brighter, more energized singing. Lower states settle into something calmer and deeper.

I kept building. A sawtooth bass marked time, changing pitch every half rotation of the Sun so the listener always knew where they were in the cycle. The helium-to-oxygen ratio drove a high-frequency shimmer, and when a CME erupts in the data, the entire scaffold responds. The wind distorts, the voices surge, and the reverb swells to fill the room, creating a sudden, vast expansion.

With this approach, researchers could close their eyes and track complex interactions between eight solar wind data parameters. The sonification was effectively communicating the data, and the work was gaining traction. It was featured on National Public Radio (NPR) and presented at the International Conference on Auditory Display.5 However, parameter mapping had yet to reveal anything new about the data. For that, I’d need a fundamentally different approach.

## THE HUM

The first time I heard the hum was in a coffee shop on a chilly January day in Ann Arbor, Michigan. It was there in the solar wind velocity, in the charge states, faint in some parameters, unmistakable in others. I initially assumed I’d made an error in my calculations. I was using Max/MSP (a programming language optimized for real-time signal processing) to write the solar wind data directly to audio buffers. I pressed play and it was there, clear as day: the Sun was humming.

It was time to check the math: 50,893 data samples gathered across 11.6 years, mapping to ~1.3 s of audio at CD-quality 44.1 kHz. At that speed, a day goes by in less than a millisecond. To confirm the frequency of the hum, I generated a sinusoidal waveform, the most fundamental waveform as it has no overtones, and swept it up until the two frequencies matched. That hum I was hearing was sitting at 137.5 Hz.

Converting that number back to the original sampling rate produced a number I recognized: 26.4 days. The solar synodic rotation period. The Sun rotates at different speeds at the poles than the equator, and “synodic” refers to the equatorial rotation speed. I was listening to the rotation of the Sun in data gathered by a satellite sitting at L1, the gravitational saddle point between the Earth and the Sun, and I was hearing harmonics in the data. But how? [see Figure 3(a) and (b)] When a single feature persists across multiple solar rotations, it sends a stream of solar wind that arrives at ACE every 26 days. Over a long enough time, this periodic signal emerges as a frequency within the data.

As the field becomes increasingly coherent, the spherical harmonics of the solar magnetic field organize the solar surface into symmetric regions—features on opposite sides, then equally spaced in thirds, fourths, and fifths, continuing up through the higher orders of the harmonic series [see Figure 3(c)]. Above the 137.5 Hz fundamental, I was hearing partials at 275 and 412.5 Hz, corresponding to periodicities of 13.5 and 9 days in the original data. During the most coherent phase, the Sun was humming a musical third, rising to the fifth, and dropping back down to the third again. The harmonic progression of the solar cycle itself was audible across a decade of ACE data.

With 30 data parameters rendered to a folder, I could arrow-key rapidly between them. The hum was present in most, but the harmonics were not. They rang out clearly in the carbon charge states C6+ and C4+, and were absent in C5+. Up to that point, nobody on the team had been talking about carbon. This was something I needed to bring to the group.

## THE STORY OF CARBON

Enrico Landi kept his field notes in meticulously organized notebooks in his office in the Space Research Building. If a major film production company were casting the role of “Italian Solar Physicist,” he would land the part. Hands down. He was sitting across from me at the end of a research group meeting, the moment when Thomas asked if there was anything else to share before we wrap up. I paused, then leaned in. We’d been focused on oxygen for years, but I’d been hearing something in the carbon data. The hum was there, strong and clear, and above it the harmonics were ringing out in C⁶⁺ and C⁴⁺.

I spoke. The room went quiet for a moment, and then Enrico chimed in. He was one of the four originators of CHIANTI, the atomic physics database that has become the gold standard for analyzing solar spectra. If there were a signal hiding in carbon charge states, he would be the person in the room best equipped to find it. He understood the potential in what I was hearing, and he wanted to dig in.

*FIGURE 3. (a) Spectrogram of audified C6+/C4+ ratio (2000– 2010) with harmonics of solar rotation marked. (b) Power spectrum showing peaks at the fundamental and overtones. (c) Corresponding spherical harmonics. (d) Solar and Heliospheric Observatory (SOHO) synoptic map confirming three spatially distributed coronal holes.*

I built an interface in Max/MSP to filter the audified data in real time and compare charge states side by side. Over the next several months, Enrico and I traced the spectral signatures back through the atomic physics. Ion abundance ratios “freeze in” close to the Sun: as the solar wind accelerates outward, the plasma thins so rapidly that ions stop exchanging electrons, locking in a snapshot of the coronal temperature at their point of origin like a fossil pressed into rock. Scientists had been reading these fossils through oxygen for over a decade. But carbon is sensitive across a wider range of temperatures than oxygen, and more effectively resolves the signatures of long-lived coronal holes [see Figure 3(d)] that drive the harmonics I had been hearing. What I heard as a difference in timbre was a difference in sensitivity: The C⁶⁺/C⁴⁺ ratio was more sensitive than the oxygen ratios the field had relied on.

The findings were published in the Astrophysical Journal in January 2012,6 and became the centerpiece of a NASA Harriet G. Jenkins Predoctoral Fellowship. I’d shown Thomas something new, but several open questions remained: What does audification add? Could others be trained to do this work? Or had we just gotten lucky?

## AUDIFICATION TO THE TEST

A new advisor stepped in. Sile O’Modhrain had a Ph.D. from Stanford’s Center for Computer Research in Music and Acoustics focused on haptics and multisensory design, and she knew how to turn a hunch into a controlled experiment. Our early studies at Michigan confirmed that the ear and the eye were finding the same things,7 and that the ear pulled ahead July/August 2026 IEEE Computer Graphics and Applications. 5 as signals got quieter and data got messier.6 But we were still working with synthesized tones. It was time to head to NASA Goddard Space Flight Center.

We gave eight heliophysicists real magnetometer data, headphones, and a simple instruction: tell us what you find. They described the solar wind as “sailing,” “a flag waving in the wind,” and “crunching snow.” When a slow wind transient swept through one of the datasets, a band of rising spectral power that had gone unnoticed on the spectrogram, one participant who caught it said it sounded like “a storm outside.” Every auditory participant identified that transient. No visual participant did. Across the board, the ear caught four times more anomalies than the eye.4

Next, we went after a harder target: low-frequency wave storms (LFWS), protons spiraling around magnetic field lines so quickly they radiate electromagnetic waves in their wake. These waves are one of the prime suspects in an 80-year-old mystery: why the Sun’s corona is millions of degrees hotter than its surface. On a spectrogram, they look like faint smudges. Through headphones, they whoosh and whirl and swirl. We trained 20 scientists to find them in Wind satellite data. Eyes alone caught less than half. Eyes and ears together caught four out of five.

Then the scientists started hearing ghosts. A handful of regions were flagged by listeners that weren’t on the answer key; we sent these back to them for another round of analysis. The expert confirmed that four contained real wave activity, and the fifth was a cyclotron wave storm buried in turbulence so heavy its boundaries dissolved into the background of the spectrogram. The listeners hadn’t made mistakes. They’d identified wave activity the expert missed.

When seven out of 10 listeners agreed something was there, they were almost always right, capturing 82% of all wave storm activity (see Figure 4). The same threshold applied to visual analysis captured 17%.4

*FIGURE 4. Expert-identified LFWS regions (black) are compared against visual-only (red) and multimodal (blue) participant markings in Wind Magnetometer data.*

In total, 20 scientists with 1 h of training and a pair of headphones had outperformed the standard analytical tool in the field, finding things the expert had missed. But these were still curated datasets, bounded tasks. The Wind spacecraft had been recording the magnetic field at 11 samples per second since 1994. Terabytes of data sitting in NASA’s archives, just waiting for someone to dust off the records and press play.

## THE MOTHER OF ALL WHOOSHES

I pulled three full years of Wind data: 2005, 2007, and 2008. A billion data points in total. Each month compressed into a few minutes of audio. I scrubbed through iZotope RX with studio headphones on, dropping markers every time something caught my ear. Whooshes. Warbles. Sizzles. Sharp chirps that cut through the broadband haze. Some events barely whispered above the turbulence. Others rang out like a bell in a silent room. I scored them 1 through 5 and kept moving. By the time I finished, the catalogue held over 500 events across three years of solar wind.

Lan Jian, a solar physicist at Goddard who had spent years cataloguing these wave storms, ran the validation. The automated search algorithms in use at the time had caught four to five times fewer events,7 and Jian found that audification sped the process up by a factor of 10 or more.8 One event stood out above the rest. I’d labeled it “the Mother of All Whooshes.” The background turbulence dropped out completely, a pristine silence, and then the waves arose, long and unmistakable, swirling through the data like wind through a canyon. Rob Wicks, a plasma physicist at Goddard, traced what was happening: a beam of protons blasting through the solar wind, so dense it was shaking the magnetic field and radiating waves as it flew. We published the results in the Astrophysical Journal,9 another clue in the 80-year-old mystery.

We’d shown, once again, that the ear catches what traditional methods overlook. We’d demonstrated that audification is a teachable skill. I’d pulled three years of satellite data off the shelf, dropped the needle, listened through nearly a billion data points and found gold. NASA’s archive held records spanning decades, across dozens of missions, and the catalog was growing every day. More ears were about to start perking up.

## THE REVERSE HARP

Martin Archer, space physicist by day and Kiss FM radio DJ by night, taught high school students to listen to magnetospheric data at Imperial College London. They discovered long-lasting wave events that had eluded standard analysis.10 They were not trained scientists or seasoned analysts, yet they contributed to a peer-reviewed discovery. The method worked.

Mike Hartinger, a heliophysicist at the Space Science Institute and a collaborator on that study, saw the potential to scale it up. He’d spent years studying the vibrations of Earth’s magnetic field lines, waves so low in frequency that no human ear could detect them without help. In November 2023, he and I sat down with NASA podcast host Padi Boyd to talk about Heliophysics Audified: Resonances in Plasmas, or HARP. I’d brought a producer’s ear to the project, refining the interface and onboarding so that volunteers could hear into the data the way a trained analyst would.

On the podcast, Mike explained the name. Earth's magnetic field lines behave like the strings of a harp: short and high-pitched near the planet, long and low farther out. NASA’s Time History of Events and Macroscale Interactions during Substorms (THEMIS) spacecraft, sweeping through the magnetosphere, runs a finger across the instrument. The data sounds like what the physics predicts: a descending glissando, pitch falling as the spacecraft moves outward through longer field lines.

Over 1800 volunteers took part in the HARP study, marking wave events and describing what they heard. They produced over 10,000 marks, and 12.6% of those marks followed an unexpected pattern: pitch rising with distance instead of falling. The volunteers were hearing a reverse harp: waves trapped along magnetic field lines, vibrating in place like a plucked string, but with frequency increasing where theory said it should decrease. A new phenomenon, discovered not by a single expert but by hundreds of human ears.11

On the podcast, I hummed along with the rotational hum of the Sun, tracing the harmonics I’d first heard in that Ann Arbor coffee shop. Padi joined in. For a moment, it was an unlikely trio: a scientist, a podcast host, and a star. It was almost as unlikely as a global ice cream brand commissioning music from the Sun.

## ICE CREAM SPACE MUSIC

The e-mail subject line read "Magnum Ice Cream Partnership Opportunity,” and it sounded so absurd that I almost didn’t open it. I’m glad that I did. Over the following months I met with the creative team at Golin and Big Sync to discuss the concept: a collaboration between the Sun and a pop star. They lined up JVKE, whose track “Golden Hour” had already gone platinum, and electronic producer Alex Metric for the production. I knew Alex’s "Head Straight" from the FIFA 10 soundtrack and was excited to dig in.

Over the years of audifying the solar wind, I’d built a collection of favorite sounds, moments where the data did something I knew I’d want to hear again. A high-frequency wave mode that sizzled just right became a hi-hat. A low-frequency resonance with the right punch became a snare. I sent Alex the collection as a sample pack: atmospheric beds, percussive hits, effects, Serum wavetable presets loaded with solar wind spectra.

As the remix opens, we’re immersed in 60 years of audified solar wind data. Underneath it all, there it is: the hum. Five solar cycles rising and falling across six decades, the same pulse from that Ann Arbor coffee shop. In the bridge, JVKE sings “I was all alone” supported by a rising event from the HARP citizen science project, the same kind volunteers were identifying in THEMIS data. The rising tone sweeping into the final chorus is an organ built from binary star data. When JVKE sings “you slow down tiiime,” the pitch drops, decelerating the orbital period of two stars circling each other. Physics and lyrics, perfectly aligned.

After the first chorus, the beat drops out. What rises in its place is the Mother of All Whooshes, the same July/August 2026 IEEE Computer Graphics and Applications. 7 wave storm that emerged from silence years earlier, now played 100 million times on TikTok.

## PRESS PLAY

The solar sample pack is available to download.12 You too can load these sounds into a sampler and build a beat from the Sun. Through SONARA, Sounds of NASA Research Activated, we’re proposing to bring sonified heliophysics data into planetariums, classrooms, and studios, with a web-based sequencer enabling anyone to create their own space music.13

*FIGURE 5. SDO imagery across multiple wavelengths, with audio spectrograms derived from the visual data (L and R).*

Not all data arrive as a waveform. With visual artist Simon Alexander Adams, I’m exploring a new approach to Solar Dynamics Observatory (SDO) data: breaking the solar surface into 16 quadrants and using the brightness of each region to sculpt the frequency spectrum (see Figure 5).14 More than 500 audio channels are collapsed to spatialized output. The result: we can track active regions as they rotate around the Sun.

Audification is now integrated into the OpenSpace visualization platform, where PSP’s magnetometers can be heard as the spacecraft navigates through the corona. We’ve also mapped the four Magnetospheric Multiscale Mission (MMS) spacecraft to a binaural sound field matching their tetrahedral formation, so that magnetic reconnection events unfold around a listener while wearing headphones.15 At spaceweather.now.audio, data from 12 NASA spacecraft are available to explore in a browser. Load a dataset, dive into the spectrogram, and when something catches your ear, annotate it and share a link.

My latest research investigates how plasma waves reshape Earth’s radiation belts,16 and in collaboration with Jaye Verniero at NASA Goddard Space Flight Center, we’re exploring the complex nature of the heliospheric current sheet, including 3-D sonification in virtual reality.

The terrain is vast and open. Volcanoes. Ocean currents. Brainwaves. And now, breath. With Breathscape, we’re combining sonified solar wind with respiratory biofeedback, turning the Sun’s rhythms into a meditative experience you can breathe. Any system that generates data is a system waiting to be heard, and there’s no telling what we’ll hear next. If you could listen to anything in the whole universe, what would you press play on first?

## ACKNOWLEDGMENTS

The author would like to thank Kelly Snook, Bobby Candey, Jason Gilbert, Sue Lepri, and the entire SHRG, Aaron Roberts, Lynn Wilson, Dean Pesnell, Barbara Thompson, Adam Szabo, Emmanuel Masongsong, Kate Meredith, Micah Lewis, and his supportive friends and family.

## REFERENCES

1. O. M. Romeo et al., "Near-sun in situ and remote-sensing observations of a CME and its effect on the heliospheric current sheet," Astrophys. J., vol. 954, 2023, Art. no. 168.

2. NASA, "Listen to SPACE! Transforming heliophysics data into sound," YouTube, Jan. 21, 2025. [Online]. Available: https://www.youtube.com/watch?v=j9A2MTB9gl0

3. H. A. Salinas et al., "MMS observations of Lion roars with higher order harmonic whistler waves inside Earth's magnetosheath," J. Geophys. Res.: Space Phys., vol. 131, 2026, Art. no. e2025JA034403.

4. R. L. Alexander et al., "Sonification of ACE level 2 Solar wind data," in Proc. 16th Int. Conf. Auditory Display (ICAD), Washington, DC, USA, 2010.

5. E. Landi et al., "Carbon ionization stages as a diagnostic of the solar wind," Astrophys. J., vol. 744, 2012, Art. no. 100.

6. R. L. Alexander et al., "The bird's ear view of space physics: Audification as a tool for the spectral analysis of time series data," JGR Space Phys, vol. 119, pp. 5259– 5271, 2014.

7. R. L. Alexander, "The bird's ear view of space physics: Audification for the spectral analysis of heliospheric time series data," Ph.D. Dissertation., Dept. Integrative Systems + Design, College Eng., Univ. Mich., Ann Arbor, MI, USA, 2015.

8. "Now hear this," Economist, Mar. 19, 2016. [Online]. Available: https://www.economist.com/science-and-technology/2016/03/19/now-hear-this

9. R. T. Wicks et al., "A proton-cyclotron wave storm generated by unstable proton distribution functions in the solar wind," Astrophys. J., vol. 819, 2016, Art. no. 6.

10. M. O. Archer et al., "First results from sonification and exploratory citizen science of magnetospheric ULF waves," Space Weather, vol. 16, no. 11, pp. 1753–1769, 2018.

11. M. D. Hartinger et al., "Inverted radial Alfvén Continua: First results from heliophysics audified: Resonances in Plasmas," Front. Astron. Space Sci., vol. 13, 2026.

12. R. L. Alexander, "Solar sample Pack I," Zenodo, 2026, doi: 10.5281/zenodo.20171838.

13. SONARA. (2026). [Online]. Available: https://sonara.now.audio/

14. R. L. Alexander, "SDO Sonification," 2024. [Online]. Available: https://spaceweather.now.audio/SDO_Sonification

15. K. Collins, R. L. Alexander, J. Verniero, and R. M. Candey, "Auralization of magnetic multiscale satellite data: Toward integrated audification in space science," in Proc. 29th Int. Conf. Auditory Display, 2024.

16. CHIRP. 2026. [Online]. Available: https://lasp.colorado.edu/chirp/home ROBERT L. ALEXANDER is an affiliate research scientist at the Space Science Institute, Boulder, CO 80301 USA and a fellow at the Arthur C. Clarke Center for Human Imagination, UC San Diego, La Jolla, CA USA. Alexander received his Ph.D. degree in design science from the University of Michigan College of Engineering, Ann Arbor, MI, USA. Contact him at robert@auralab.io.

July/August 2026 IEEE Computer Graphics and Applications. 9
