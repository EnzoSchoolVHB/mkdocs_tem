# Documentation CTF Root-Me

## TC1 - BTS-SIO Niveau 1 (Tronc commun)

* [Challenges 5 Points]()
    * Javascript - Authentification
    * Javascript - Source
    * HTML - Code source
    * TELNET - authentification
    * Hash - Message Digest 5


## Challenges 5 Points

### Javascript - Authentification

Dans le code **JavaScript** de a page, on a les identifiant en claire.   
```js
if (pseudo=="4dm1n" && password=="sh.org")
```

### Javascript - Source

Quand on ouvre la page on a une pop-up qui nous demande un password. Le mot de passe est cacher dans le JS.
```js
pass=prompt("Entrez le mot de passe / Enter password");
		if ( pass == "123456azerty" ) 
```

### HTML - Code source

Le mot de passe est marqué dans le code html en commentaire.

````html
<!--
    Je crois que c'est vraiment trop simple là It's really too easy ! password : nZ^&@q5&sjJHev0
-->
````

### TELNET - authentification

Le mot de passe pour ce connecter à TELNET est écris en claire dans une trame réseau. 

### Hash - Message Digest 5

On avait un fichier qui contient un mot de passe crypter. Il suffisait de trouvé en qu'elle hash le mot de passe étais crypter puis le décrypter.

