<script setup lang="ts">
import Section from '@/components/Section.vue'
import TitleWidget from '@/components/TitleWidget.vue'
</script>

<template>
  <TitleWidget title="Dokumentation" />

  <Section title="Wie ist die Objekthierarchie einer Liegenschaft aufgebaut?">
    <h3>Project = Liegenschaft</h3>
    <p>
      Eine Liegenschaft bezeichnet ein oder mehrere Grundstücke,
      die wiederum mit ein oder mehreren Gebäuden oder Anlagen bebaut sind
      und meist eine funktionale Einheit bilden.
    </p>
    <h3>Property = Grundstück</h3>
    <p>
      Ein Grundstück ist ein räumlich abgegrenzter Teil, der eine bestimmte Größe besitzt und
      einer bestimmten Wirtschaftsart und Lage zugeordnet ist.
      Ein Grundstück entspricht genau einem Eintrag im Bestandsverzeichnis des Grundbuches.
      Daher können mehrere Grundstücke einer Liegenschaft auch die identische Grundbuch Blattnummer besitzen.
    </p>
    <h3>Site = Außenanlage</h3>
    <p>
      Eine Außenanlage ist ein Teil eines Grundstücks, das sich im Außenbereich befindet und
      nicht Bestandteil eines Gebäudes ist. Zu den Außenanlagen gehören unter anderem Stellplätze,
      Zufahrten, Liegeplätze, Gartenanlagen, Grünflächen oder andere Außenflächen,
      die keine Wohn- oder Nutzflächen besitzen und als Teilmengen der Grundstücksfläche bewirtschaftet werden.
    </p>
    <h3>Building = Gebäude</h3>
    <p>
      Ein Gebäude ist ein Bauwerk auf einem Grundstück, das Räume einschließt,
      betreten werden kann und dem Aufenthalt von Menschen, Tieren oder der Lagerung von Sachen
      als Wohn-, Gewerbe- oder Nutzflächen dient. Es können mehrere Gebäude
      auf einem Grundstück errichtet sein und als eine Einheit bewirtschaftet werden.
      Grundsätzlich besteht ein Gebäude aus ein oder mehreren Etagen mit oder ohne Keller.
      Das Gebäude ist untergliedert in diverse Einheiten, die sich im Keller,
      in den Etagen oder auch im Dachgeschoss befinden können.
    </p>
    <h3>Apartment = Wohnung</h3>
    <p>
      Eine Wohnung ist ein umschlossener Raum oder eine Flucht aus mehreren Räumen innerhalb eines Gebäudes,
      die zu Wohnzwecken laut Baugenehmigung verwendet werden darf.
      Eine Wohnung besteht daher aus Wohn- und Nutzfläche, die sich nach der
      <a href="https://www.gesetze-im-internet.de/woflv/BJNR234610003.html"
         class="underline hover:decoration-green-600" target="_blank">
        Verordnung zur Berechnung der Wohnfläche (Wohnflächenverordnung - WoFlV)
      </a>
      berechnet.
    </p>
    <h3>Storage(ehem. Garage) = Nebennutzungsraum</h3>
    <p>
      Ein Nebennutzungsraum oder auch Zubehörraum ist eine meist abschließbare und durch feste Wände umschlossene
      Abstellmöglichkeit innerhalb eines Gebäudes, die ausschließlich aus Nutzfläche besteht
      und nicht zur Wohnfläche gehört entsprechend der
      <a href="https://www.gesetze-im-internet.de/woflv/BJNR234610003.html"
         class="underline hover:decoration-green-600" target="_blank">
        Verordnung zur Berechnung der Wohnfläche (Wohnflächenverordnung - WoFlV)
      </a>.
      Hierzu zählen Garagen, Stellplätze in Tiefgaragen, Kellerräume, Waschküchen, Abstell-, Hobby- oder Lagerräume.
    </p>
    <h3>Commercial = Gewerberäume</h3>
    <p>
      Ein Gewerbe bestehend aus mehreren Gewerberäumen ist ein Laden oder ein Zusammenschluss mehrerer Räume innerhalb eines Gebäudes,
      die ausschließlich oder vorwiegend der Unterbringung von Industrie- oder Gewerbebetrieben dient.
      Gewerberäume werden nach der
      <a href="https://www.dinmedia.de/de/norm/din-277/342217323"
         class="underline hover:decoration-green-600" target="_blank">
        DIN 277:2021-08 Norm für Grundflächen und Rauminhalte im Hochbau
      </a>
      berechnet und
      bestehen daher aus Nutzungsfläche (NUF), Verkehrsfläche (VF) und Technikfläche (TF).
      Insgesamt ergibt sich aus der Summe dieser Flächen die Netto-Raumfläche (NRF) einer Gewerbeeinheit.
      Eine Aufteilung der Nutzungsfläche in die sieben Unterkategorien nach ihren Funktion kann
      in der Beschreibung der Gewerbeeinheit angegeben werden.
    </p>
  </Section>

  <div class="github-section">
    <p class="text-base">
      Weitere Details finden Sie in unseren
      <a href="https://github.com/remsfal/remsfal/issues"
         class="underline hover:decoration-green-600" target="_blank">
        GitHub Issues
      </a>
    </p>
  </div>
</template>

<style scoped>
.github-section {
  text-align: center;
  margin-top: 40px;
  padding: 20px;
  background: var(--vt-c-black);
  border-radius: 8px;
}
</style>
