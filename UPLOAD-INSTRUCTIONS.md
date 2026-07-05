# Kako da postavis novu verziju (jednom podesavanje, posle samo upload)

## Deo A — jednokratno podesavanje (5 min)

1. Otvori repo na GitHub-u → **Add file → Create new file**
2. U polje za ime ukucaj TACNO:  `.github/workflows/deploy.yml`
   (GitHub ce sam napraviti foldere kad ukucas kose crte)
3. Nalepi sadrzaj fajla `deploy.yml` iz ovog zip-a → **Commit changes**
4. Idi na **Settings → Pages** → pod "Build and deployment" → **Source** promeni na **GitHub Actions**
5. Gotovo. Od sada svaki commit na main automatski objavljuje sajt — bez Jekyll-a, bez .nojekyll zavisnosti.

## Deo B — svaka sledeca izmena

1. Otvori `index.html` u repo-u → olovka (ili Add file → Upload files preko postojeceg)
2. Zameni sadrzaj novim `index.html` iz zip-a → **Commit changes**
3. **Actions** tab → sacekaj zelenu kvacicu (~1 min) → isti link je azuriran
   (hard refresh: Cmd+Shift+R ako ne vidis promenu)

## Ako nesto padne

- Actions → klikni crveni run → crveni korak → poruka na dnu loga kaze tacan uzrok.
- Posalji screenshot te poruke Claude-u.
