// Liste des dons
let donations = [];

// Fonction pour faire un don
function donate(amount) {
  // Lien Awoopay prêt à utiliser
  const paymentLink = `https://pay.awoopay.com/test123?amount=${amount}`;
  
  // Ouvre le lien dans le navigateur
  window.open(paymentLink, "_blank");

  // Ajouter le don dans le tableau
  donations.unshift({ name: "Donateur anonyme", amount });

  // Afficher les derniers dons
  renderDonations();
}

// Afficher les dons
function renderDonations() {
  const container = document.getElementById("donations");
  container.innerHTML = "";
  donations.forEach(d => {
    const div = document.createElement("div");
    div.innerHTML = `${d.name} : ${d.amount} FCFA`;
    container.appendChild(div);
  });
}
