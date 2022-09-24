<template>
  <Nav />
  <main class="container">
    <h1>
      <a href="/"
        ><img
          class="mx-auto d-block img-fluid"
          src="~/assets/images/arcah1.jpg"
          alt="Arca Musica"
      /></a>
    </h1>
    <section class="row bouton gap-3 mx-0">
      <a
        href="https://forms.gle/1XjUhJyopYbtY3SJ9"
        role="button"
        type="button"
        class="btn btn-dark col"
      >
        Demander un cours d'essai
      </a>
      <a
        href="/coursettarifs"
        role="button"
        type="button"
        class="btn btn-dark col"
        >Nos Cours</a
      >
      <a
        href="/presentation"
        role="button"
        type="button"
        class="btn btn-dark col"
        >En savoir plus</a
      >
    </section>
    <section class="row identite p-1">
      <h2 class="text-center p-4">Découvrez votre école de musique</h2>

      <p class="col-sm">
        Depuis que nous avons ouvert nos portes en septembre 2019, nous nous
        efforçons d'aider nos élèves à poursuivre un chemin qui les inspire.
        Grâce à nos professeurs passionnés, nos élèves investis, nous sommes
        fiers de l’éducation, des conseils et du réseau que vous trouverez chez
        nous.
      </p>
      <p class="col-sm">
        Arca Musica propose une méthode d'apprentissage personnalisée, qui
        favorise l'épanouissement et l'apprentissage des étudiants, et qui
        encourage les esprits créatifs à se dépasser.
      </p>
    </section>
  </main>
  <Footer />
</template>

<style scoped>
</style>

<script setup >
// import { PDF } from "swissqrbill/pdf";
// import { mm2pt } from "swissqrbill/utils";

// const data = {
//   currency: "CHF",
//   amount: 2000,
//   reference: "210000000003139471430009017",
//   creditor: {
//     name: "Robert Schneider AG",
//     address: "Route d'Yverdon",
//     buildingNumber: "8",
//     zip: 2501,
//     city: "Biel",
//     account: "CH4431999123000889012",
//     country: "CH",
//   },
//   debtor: {
//     name: "Pia-Maria Rutschmann-Schnyder",
//     address: "Grosse Marktgasse",
//     buildingNumber: "28",
//     zip: 9400,
//     city: "Rorschach",
//     country: "CH",
//   },
// };

// const pdf = new PDF(
//   data,
//   "Complete-qrbill.pdf",
//   { language: "FR", autoGenerate: false, size: "A4" },
//   () => {
//     console.log("PDF has been successfully created.");
//   }
// );
// pdf.fontSize(12);
// pdf.fillColor("black");
// pdf.font("Helvetica");
// pdf.text(
//   data.creditor.name +
//     "\n" +
//     data.creditor.address +
//     "\n" +
//     data.creditor.zip +
//     " " +
//     data.creditor.city,
//   mm2pt(20),
//   mm2pt(35),
//   {
//     width: mm2pt(100),
//     height: mm2pt(50),
//     align: "left",
//   }
// );

// //-- Add debtor address

// pdf.fontSize(12);
// pdf.font("Helvetica");
// pdf.text(
//   data.debtor.name +
//     "\n" +
//     data.debtor.address +
//     "\n" +
//     data.debtor.zip +
//     " " +
//     data.debtor.city,
//   mm2pt(130),
//   mm2pt(60),
//   {
//     width: mm2pt(70),
//     height: mm2pt(50),
//     align: "left",
//   }
// );

// //-- Add title

// pdf.fontSize(14);
// pdf.font("Helvetica-Bold");
// pdf.text("Rechnung Nr. 1071672", mm2pt(20), mm2pt(100), {
//   width: mm2pt(170),
//   align: "left",
// });

// const date = new Date();

// pdf.fontSize(11);
// pdf.font("Helvetica");
// pdf.text(
//   "Musterstadt " +
//     date.getDate() +
//     "." +
//     (date.getMonth() + 1) +
//     "." +
//     date.getFullYear(),
//   {
//     width: mm2pt(170),
//     align: "right",
//   }
// );

// //-- Add table

// const table = {
//   width: mm2pt(170),
//   rows: [
//     {
//       height: 30,
//       fillColor: "#ECF0F1",
//       columns: [
//         {
//           text: "Position",
//           width: mm2pt(20),
//         },
//         {
//           text: "Anzahl",
//           width: mm2pt(20),
//         },
//         {
//           text: "Bezeichnung",
//         },
//         {
//           text: "Total",
//           width: mm2pt(30),
//         },
//       ],
//     },
//     {
//       columns: [
//         {
//           text: "1",
//           width: mm2pt(20),
//         },
//         {
//           text: "14 Std.",
//           width: mm2pt(20),
//         },
//         {
//           text: "Programmierung SwissQRBill",
//         },
//         {
//           text: "CHF 1'540.00",
//           width: mm2pt(30),
//         },
//       ],
//     },
//     {
//       columns: [
//         {
//           text: "2",
//           width: mm2pt(20),
//         },
//         {
//           text: "8 Std.",
//           width: mm2pt(20),
//         },
//         {
//           text: "Dokumentation",
//         },
//         {
//           text: "CHF 880.00",
//           width: mm2pt(30),
//         },
//       ],
//     },
//     {
//       height: 40,
//       columns: [
//         {
//           text: "",
//           width: mm2pt(20),
//         },
//         {
//           text: "",
//           width: mm2pt(20),
//         },
//         {
//           text: "Summe",
//           font: "Helvetica-Bold",
//         },
//         {
//           text: "CHF 2'420.00",
//           font: "Helvetica-Bold",
//           width: mm2pt(30),
//         },
//       ],
//     },
//     {
//       columns: [
//         {
//           text: "",
//           width: mm2pt(20),
//         },
//         {
//           text: "",
//           width: mm2pt(20),
//         },
//         {
//           text: "MwSt.",
//         },
//         {
//           text: "7.7%",
//           width: mm2pt(30),
//         },
//       ],
//     },
//     {
//       columns: [
//         {
//           text: "",
//           width: mm2pt(20),
//         },
//         {
//           text: "",
//           width: mm2pt(20),
//         },
//         {
//           text: "MwSt. Betrag",
//         },
//         {
//           text: "CHF 186.35",
//           width: mm2pt(30),
//         },
//       ],
//     },
//     {
//       height: 40,
//       columns: [
//         {
//           text: "",
//           width: mm2pt(20),
//         },
//         {
//           text: "",
//           width: mm2pt(20),
//         },
//         {
//           text: "Rechnungstotal",
//           font: "Helvetica-Bold",
//         },
//         {
//           text: "CHF 2'606.35",
//           width: mm2pt(30),
//           font: "Helvetica-Bold",
//         },
//       ],
//     },
//   ],
// };

// pdf.addTable(table);

// //-- Add QR slip

// pdf.addQRBill();

// //-- Finalize the document

// pdf.end();
</script>
