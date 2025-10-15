## 📈 Progress
Today, I researched semiconductor and photodetector fundamentals for selecting a photodectector. I also began to review microelectronics design for the analog front-end.

---

### Semiconductor Basics
Semiconductor devices rely on what is known as the P–N junction. To create one, we start with a semiconductor such as silicon, whose crystalline lattice has four valence electrons. This allows it to behave as either a conductor or insulator depending on conditions. One region of the silicon is doped with a pentavalent impurity (such as phosphorus, which has five valence electrons). This produces an N-type region with an excess of free electrons as majority carriers. The other region is doped with a trivalent impurity (such as boron, with three valence electrons), creating a P-type region with electron “holes” (vacancies in the lattice that act as positive charge carriers) as the majority carriers. When the P-type and N-type materials are joined, a diffusion process occurs: electrons from the N-region migrate into the P-region to fill holes, and holes from the P-region migrate into the N-region. This transfer leaves behind immobile ionized donor atoms (positively charged in the N-region) and ionized acceptor atoms (negatively charged in the P-region). These fixed charges create an internal electric field across the junction. As diffusion continues, this field builds until it counteracts further carrier motion, and the system reaches equilibrium. The region around the interface becomes the depletion layer, nearly free of mobile charge carriers. The N-side is left with a net positive charge due to uncovered donor ions, while the P-side is left with a net negative charge due to uncovered acceptor ions. This results in a built-in electric field directed from the positive N-side toward the negative P-side, producing a built-in potential barrier (the contact potential). To drive current across the junction, an external voltage must be applied that either reinforces or opposes this barrier (forward bias vs. reverse bias). In a photodiode, when incident photons with energy greater than the silicon bandgap strike the depletion region, they excite electrons from the valence band into the conduction band, generating electron–hole pairs. The built-in electric field immediately sweeps electrons toward the N-side and holes toward the P-side, producing a measurable photocurrent. This process of conversion of absorbed light into electrical energy is known as the photovoltaic effect. It forms the basis for devices such as solar cells and light sensors.

For our portable fluorescein reader, I selected a Hamamatsu S1223 PIN photodiode. It has good responsivity near 515 nm, a low dark current, low capacitance, and a PCB/TO-style package for easy alignment. 

## 🧩 Challenges
Today's challenege was researching the analog front-end of the device to be optimized based on the requirements. I want to explore the technical characteristics of the electronics in depth before I commit to anything.

## 🥅 Goals
Tomorrow, I would like to finish the analog circuit design, including any calculations and diagrams.

