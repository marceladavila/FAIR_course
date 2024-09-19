<!--
title: "Liascript Presentations"

import: https://raw.githubusercontent.com/LiaScript/CodeRunner/master/README.md
        https://raw.githubusercontent.com/LiaTemplates/BeforeAndAfter/0.0.1/README.md

icon:   https://tess.elixir-europe.org/assets/elixir/elixir-tess-219b707c4912e9c46c917a24ce72b464ec9f2fd56ce03dbcee8b2f6b9ac98a44.svg

link:   https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css
        https://fonts.googleapis.com/css?family=Lato:400,400italic,700
        style.css

@runR: @LIA.eval(`["main.R"]`, `none`, `Rscript main.R`)

@JSONLD
<script run-once>
  let json = @0 

  const script = document.createElement('script');
  script.type = 'application/ld+json';
  script.text = JSON.stringify(json);

  document.head.appendChild(script);

  // this is only needed to prevent and output,
  // as long as the result of a script is undefined,
  // it is not shown or rendered within LiaScript
  console.debug("added json to head")
</script>
@end


link:   https://unpkg.com/leaflet@1.9.4/dist/leaflet.css
script: https://unpkg.com/leaflet@1.9.4/dist/leaflet.js


{
  "@context": "https://schema.org/",
  "@type": "LearningResource",
  "@id": "https://dev.tess.elixir-europe.org/events/easy-with-bioinformatics",
  "http://purl.org/dc/terms/conformsTo": {
    "@type": "CreativeWork",
    "@id": "https://bioschemas.org/profiles/TrainingMaterial/1.0-RELEASE"
  },
  "description": "This is a super short exercise to showcase the importance of bioinformatics",
  "keywords": "Bioinformatics",
  "name": "It is easier with Bioinformatics",
  "license": "https://creativecommons.org/licenses/by/4.0/",
  "educationalLevel": "beginner",
  "competencyRequired": "none",
  "teaches": [
    "Define the term Bioinformatics", 
    "Ilustrate the utility of using bioinformatics in a toy example"
  ],
  "audience": "researchers","students",
  "inLanguage": "en-US",
  "learningResourceType": [
    "tutorial"
  ],
"identifier": [
  "https://zenodo.org/doi/10.5281/zenodo.13794531"
]
  
  "author": [
    {
      "@type": "Person",
      "name": "Marcela Dávila"
    }
  ]
}

-->



# Mini-Lesson overview

## It is easier with Bioinformatics

* **Identifier:**  [ https://zenodo.org/doi/10.5281/zenodo.13784767](https://zenodo.org/doi/10.5281/zenodo.13794531)

*  This work is licensed under [Creative Commons Attribution-NonCommercial 4.0 International](https://creativecommons.org/licenses/by-nc/4.0/?ref=chooser-v1) 

*  **Author:** Marcela Dávila

* **Target Audience:** Researchers, students

* **Level:** Beginner

*  **Keywords:** Bioinformatics

* **Prerequisites:** To be able to follow this course, learners should have basic knowledge in biology or molecular biology

* **Description:** This is a super short exercise to showcase the importance of bioinformatics
 
* **Learning Outcomes:**  By the end of the course, participants will be able to:

     1. Define the term Bioinformatics 
     2. Ilustrate the utility of using bioinformatics in science today



https://liascript.github.io/course/?https://raw.githubusercontent.com/marceladavila/FAIR_course/main/README.md#1

## What is bioinformatics

## How many GATACA's do you see

```
GATACAGATAT 
CGATACACGAT
ACAGATCGACA
TACGAGATACA
```

## There are 4 

![](https://github.com/marceladavila/FAIR_course/blob/main/images/dos.png)



## And now??

![](https://github.com/marceladavila/FAIR_course/blob/main/images/tres.png)

```
GATACAGATATGATACCCCAGGGATGCAGCTAGATCGATCGATGCTAGCTGATCGTACGTCGGATACAGAT 
CGATACACGATCTACGTAGCTGACTGTACGGTGCGTAGGATATATATAGGATACAGTCAGTACGTCGGATA
ACAGATCGACAGTAGTGTACCCCGTACGTACGATACAGGTAGATACGAGATACAGACTACGAGCATACGTA
GTACGTACGACTAGCTAGGATACAGGTGTGATACAGTAGGATAGCGCTACGTACGATCGATGGTACACGAT
ACAGATACATCGTACGATGCTAGTCAGCAGAGATCATAGGATACAGTAGGACGACTGACGTACGTACGACG
GCTACGTGATGACGGATACAGTCAGCGCGTATCGAGGAAGATATATAGATAAGTAGGATACAGATGATGTG
```

## Not so easy right?

![](https://github.com/marceladavila/FAIR_course/blob/main/images/cuatro.png)

Imagine there is a video here :)

<details>
          <summary>Transcript click here</summary>

are a gregarious herd species that were domesticated from wild orcs that lived in modern Syria and Pakistan. Since their domestication, the number of cows has increased and they now have the largest biomass of any animal species on Earth. The gut floor of cows produce mephane, which is a powerful greenhouse gas. Unfortunately, increasing heat from climate change causes stress for cows and makes them more susceptible to illness, both from decreasing their appetite and increasing the number of arthropod vectors like flies and ticks. Appetite stress is a problem for cows as they have specialized physiology for eating and digestion. They even adjust their chewing depending on the time of day and the type of plant they're eating. Little is known of the life histories of many jellyfish. These pacif hunters have a complex life cycle where the medusa form butts from a polyp attached to the deep benthic sea floor. Looms occur where jellyfish, which are able to survive in warm, nutrient rich and oxygen poor water, congregate and feast on plankton and fish eggs together. Overfishing of larval jellyfish predators can result in jellyfish becoming dominant in an ecosystem. Few animals prey on mature jellyfish, and once their populations increase there may be no way for the previous balance to be restored. The global population of jellyfish is expanding as their physiology allows them to benefit from disrupted marine ecosystems, which feature few prey species, warmer water, low oxygen, and high organic matter.

</details>


## With a little coding

``` sh
% grep GATACA gataca.txt -o
GATACA
GATACA
GATACA
GATACA
GATACA
GATACA
GATACA
GATACA
GATACA
GATACA
GATACA
GATACA

% grep GATACA gataca.txt -o | wc -l
12

```
