# Kuponeo — publiczny feed kuponów

Statyczny, podpisany cyfrowo plik z treścią kuponów dla aplikacji Kuponeo.

- **Adres produkcyjny:** https://kuponeo.github.io/kuponeo-feed/feed.json
- **Format:** JSON `{ payload, sig }` — `sig` to podpis Ed25519 nad bajtami UTF-8 pola `payload`; aplikacja odrzuca plik z niepoprawnym podpisem oraz plik starszy niż już zastosowany.
- Ten plik jest jawny z założenia (pobiera go każda instalacja aplikacji). Integralności pilnuje podpis kryptograficzny, nie ukrycie.
- Historia commitów tego repozytorium stanowi rejestr tego, co i kiedy było opublikowane.
