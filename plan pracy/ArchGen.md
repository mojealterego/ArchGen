# Plan pracy — ArchGen

## Status audytu
AUDYT ZAKOŃCZONY — 2026-09-12.

## Stan faktyczny
Next.js 14/React/TypeScript z API routes, Gemini i własnym rendererem SVG. System ma generować architektury z wymagań i budżetu oraz eksportować SVG/PNG/PDF/JSON/Docker Compose. README deklaruje również wyniki benchmarków, których nie należy uznawać za potwierdzone bez reprodukcji.

## Ryzyka
- koszty chmurowe są tylko szacunkowe;
- eksport Docker wymaga walidacji bezpieczeństwa;
- endpointy generowania/eksportu potrzebują limitów i walidacji;
- brak potwierdzenia aktualności Next.js 14/Gemini.

## Priorytet
WYSOKI.

## Kolejność prac
1. Zweryfikować kod, manifest i API.
2. Dodać testy parsera wymagań i schematu architektury.
3. Walidować eksporty i nie wykonywać wygenerowanych konfiguracji automatycznie.
4. Zabezpieczyć endpointy, limity i sekrety.
5. Odtworzyć deklarowane benchmarki.
6. Spolonizować UI i dokumentację.

## Kryterium zakończenia
Schemat architektury jest walidowany, eksporty są bezpieczne, koszty są oznaczone jako estymacje, a wyniki benchmarków mają reprodukowalną metodologię.
