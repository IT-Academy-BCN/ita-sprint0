# Manual de Bones Pràctiques per a Lliuraments de Projectes  
*(Per a estudiants de desenvolupament Back-end i Front-end)*

---

## 📌 Introducció

Aquest manual unifica els criteris essencials per fer lliuraments professionals de projectes, combinant:

✅ Bones pràctiques tècniques (codi net, estructura, testing)  
✅ Gestió professional (Git, documentació, CI/CD bàsic)  
✅ Estàndards de qualitat (revisió per parells, principis SOLID/KISS/DRY)

---

## 🔧 1. Configuració del Repositori

### 1.1 Estructura Bàsica

```plaintext
projecte/
├── src/                  # Codi font
├── tests/                # Proves automàtiques  
├── .gitignore            # Fitxers exclosos  
└── README.md             # Documentació principal
```


### 1.2 Normes Git

- **Noms dels repositoris**: Descriptius i en anglès (ex. `task-manager`, no `projecte1`).
- **Commits**: Atòmics i amb missatges clars, seguint la convenció *Conventional Commits*:

```bash
git commit -m "feat: add user authentication"
git commit -m "fix: resolve login timeout error"
```
- Branques: Fer servir Gitflow (`main`, `develop`, `feature/xxx`).

## 💻 2. Qualitat del Codi

### 2.1 Principis Fonamentals

| Principi | Descripció                                  | Exemple                             |
| -------- | ------------------------------------------- | ----------------------------------- |
| KISS     | Mantingues el codi senzill i llegible       | Evita sobre-enginyeria en funcions  |
| DRY      | No repeteixis codi. Fes servir mòduls       | Extreure lògica repetida a `utils/` |
| SOLID    | (Back-end) Disseny OOP amb bones pràctiques | `Responsabilitat única` en classes  |


### 2.2 Estil i Convencions

**Front-end:**
- ✔ JS/TS: `camelCase` per a variables i funcions, `PascalCase` per a components.
- ✔ CSS: Utilitzar metodologies com `BEM`.

**Back-end:**
- ✔ Java/Python: Seguir convencions del llenguatge (`snake_case` en Python, `camelCase` en Java).

### 2.3 Funciones y Métodos

- ✔ Cuida la quantitat de línies per funció (si és més llarg, dividir).
- ✔ Utilitzar *early returns* para simplificar lógica:
    ```java
    function getUser(id) {
    if (!id) return null;  // Early return
    // Lògica principal...
    }
    ```

### 2.4 Gestió d'Errors

- **Front-end:** Mostrar feedback clar a l’usuari (ex. missatges toast)..
- **Back-end:** Utilitzar middlewares d'error i codis HTTP adequats:
    ```java
    // Exemple amb Express
    app.use((err, req, res, next) => {
    res.status(500).json({ error: "something went wrong" });
    });
    ```

## 📄 3. Documentació

### 3.1 README.md (Obligatori)

Ha d'incloure:
```html
# Nom del Projecte  
**Descripció**: Breu explicació de l'objectiu.  

## 🛠 Tecnologies  
- Frontend: React, Tailwind  
- Backend: Node.js, MongoDB  

## 🚀 Instal·lació  
1. Clonar el repositori: `git clone ...`  
2. Instal·lar dependències: `npm install`  
3. Variables d'entorn: Crear `.env` amb...  

## 📸 Demo  
[Enllaç a Vercel/Netlify] o captures de pantalla.
```

### 3.2 Comentarios en Código

Intenta evitar-los, recorda que un codi net s'autodescriu. Si els utilitzaràs, tingues en compte explicar el per què, no el què:
```java 
// ❌ Malament: "Suma a + b"
// ✅ Bé: "Necessari per calcular el total amb impostos (Llei XYZ)"
function calculateTotal(a, b) { ... }
 ```

## 🧪 4. Testing (Opcional pero Recomendado)

- Cobertura mínima: 70% per a projectes avançats

## 🔍 5. Code Review por Pares

Sempre demana una segona opinió. El codi sempre ha d'estar en un cicle de millora continua. veure instruccions a l'arxiu `code_review_p2p`

### 5.1 Checklist de Revisión

| Àrea          | Preguntes Clau                                         |
| ------------- | ------------------------------------------------------ |
| Funcionalitat | Compleix tots els requisits de l’enunciat?             |
| Codi Neteja   | Segueix els principis DRY/KISS? Té noms descriptius?   |
| Seguretat     | Hi ha dades sensibles exposades? Validació d’entrades? |


## 🚀 6. Entrega Final

Antes de entregar:
- Ejecuta tests locales
- Prueba en otro dispositivo (evita el “en mi PC funciona”)
- Actualiza el README.md con instrucciones claras


## ✨ Bonus: Consejos Pro

- Front-end: Usar herramientas como ESLint/Prettier para consistencia
- Back-end: Implementar logging básico (winston, morgan)
- DevOps Básico: Configurar GitHub Actions para tests automáticos i Deployments.

