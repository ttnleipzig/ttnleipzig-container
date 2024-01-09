---
title: Bastelrunde - 012 Build Pipeline
description: Debugging mit IoT
tags:
  - slide
  - programming
  - lorawan
type: slide
---

<style>
@import url('https://fonts.googleapis.com/css2?family=Lobster&family=Permanent+Marker&display=swap');
h1, h2 {
	font-family: 'Permanent Marker', cursive !important;
	text-shadow: 0 0 12px #000 !important;
}
</style>

<!-- slide bg="[[andrelademann_22433_constructors_build_a_futuristic_pipeline_th_13717e9c-dc02-411a-bcfb-912d36a06e31.png]]" data-auto-animate     -->

# Bastelrunde 
<!-- element style="padding-top: 30%; text-shadow: 4px 4px 2px 2px #000;" -->
## #012 GitHub Actions

<!-- element style="text-shadow: 4px 4px 2px 2px #000" -->

<!--
**Checkliste bevor es losgeht:**

- [ ] Foto gemacht
- [ ] Tweet gesendet
- [ ] Hochkant Video

-->

---

## Onboarding

1) Was ist LoRaWAN Leipzig
2) Wo wir uns befinden
3) Wo die Toiletten sind
4) Wo gibt es Getränke?

<!--
- [ ] Was ist LoRaWAN Leipzig
	- [ ] Ziele
	- [ ] Wer sind die Leute
- [ ] Wo befinden wir uns (Basislager, Kohlenstraße)
- [ ] Wo sind die Toiletten
- [ ] Wo gibt es Getränke?
-->

--

<!-- element style=" text-shadow: 4px 4px 2px 2px #000; color: #999; font-size: 1rem;" -->
sponsored by

![Thinkport](https://thinkport.digital/wp-content/uploads/elementor/thumbs/Logo_horizontral_new-q79kisryfbimg521qvcamhuu9zgajwl52ie1tm6q0s.png)
--


## Projektübersicht

1) ✅ Hardware Prototyp
2) 👩‍💻 Verbindung mit TTN
3) 👩‍💻 Automatisierte Releases auf GitHub
4) Datenverarbeitung in NodeRED
5) Datenmonitoring und Visualisierung


---
<!-- slide bg="[[vergissberlin_microcontroller_flying_through_clouds_e4ca3e11-4904-4bfb-a259-0a4fbf2dee4e.png]]" -->

<grid drag="60 30" bg="#000000cc" style="border-radius: 12px;backdrop-filter: blur(10px);" pad="1em 2em 1em 1em">

## Today

👩‍💻🧑🏼‍💻👨🏻‍💻

1) Pipeline - Wie machen das Andere (WLED)
2) Pipeline - Wie wollen wir das machen
3) Pipeline - Erster Prototyp
4) Weitere Schritte besprechen

</grid>

---
<!-- slide bg="#112" data-auto-animate -->
### Main branch (Stable branch)

> Beim setzen eines Tags wird

1) Werden die Tests durchgeführt
2) Werden automatisch die binaries gebaut
3) Automatisch eine Release page erstellt
4) Werden die Binaries automatisch zur Release page hochgeladen

--
<!-- slide bg="#111" data-auto-animate -->
![[Pasted image 20240109181349.png]]

---
<!-- slide bg="#112" data-auto-animate -->
### Feature branch

> Bei jedem commit

1) Werden die Tests durchgeführt
2) Werden binaries erstellt
3) Werden die Binaries automatisch dem dazugehörigem Ticket hochgeladen

--
<!-- slide bg="#111" data-auto-animate -->
![[Pasted image 20240109181739.png]]

---

## Off-boarding

1) 🏁 Was wir heute geschafft haben
2) 🔎 Wo man den Quellcode findet
3) 🙋‍♂️ Fragen, Nöte oder Anregungen?
4) 📆 Wann wir uns das nächste Mal treffen
5) 🫥 Nothing left behind
	- 🚪 Türen zu
	- 🗑️ Müll mitnehmen
	- 🪑 Stühle ranstellen

---

## Checkliste nach der Veranstaltung

-  Hardware zusammengesucht und eingepackt
- Nachher Foto
- Folgetermin Termin steht fest
- Hochkant Video - Zusammenfassung, Folgetermin
