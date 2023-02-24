# Klaviatura dlja ukrajins'koji latynky

Ce klaviatura dlja vykorystannja ukrajins'koji latynyci.

[![English](https://img.shields.io/badge/%F0%9F%93%84-English-blue)](readme.md)
[![Українська](https://img.shields.io/badge/%F0%9F%93%84-%D0%A3%D0%BA%D1%80%D0%B0%D1%97%D0%BD%D1%81%D1%8C%D0%BA%D0%BE%D1%8E-blue)](readme.uk.md)
[![Latynka](https://img.shields.io/badge/%F0%9F%93%84-Latynka-blue)](readme.uk@latynka.md)

Peršu rozkladku zaproponovano Maksymom Prudeusom, dyvit'sja v [Ukrajins'ka latynka (latyns'kyj alfavit): usi "za" i "proty"][latynka]. Vona ž je rozkladkoju za zamovčennjam.

```
┌─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┲━━━━━━━━━┓
│ ~   │ !   │ "   │ № § │ ₴ £ │ % ° │ ^   │ &   │ *   │ ( ̣  │ )   │ _ — │ + ± ┃ ⌫ Back  ┃
│ ' ` │ 1   │ 2 @ │ 3 # │ 4 $ │ 5 € │ 6   │ 7   │ 8   │ 9   │ 0   │ - – │ = ≠ ┃  space  ┃
┢━━━━━┷━┱───┴─┬───┴─┬───┴─┬───┴─┬───┴─┬───┴─┬───┴─┬───┴─┬───┴─┬───┴─┬───┴─┬───┺━┳━━━━━━━┫
┃       ┃ Ĝ Q │ Š W │ E   │ R ₹ │ T   │ Y   │ U   │ I   │ O   │ P   │ {   │ }   ┃ Enter ┃
┃Tab ↹  ┃ ĝ q │ š w │ e € │ r ® │ t ™ │ y ¥ │ u   │ i   │ o   │ p   │ [   │ ]   ┃   ⏎   ┃
┣━━━━━━━┻┱────┴┬────┴┬────┴┬────┴┬────┴┬────┴┬────┴┬────┴┬────┴┬────┴┬────┴┬────┺┓      ┃
┃        ┃ A   │ S   │ D   │ F   │ G   │ H   │ J   │ K   │ L ₪ │ Č   │ " “ │ |   ┃      ┃
┃Caps ⇬  ┃ a   │ s   │ d   │ f   │ g   │ h   │ j   │ k   │ l ₺ │ č   │ ' „ │ \   ┃      ┃
┣━━━━━━━━┹────┬┴────┬┴────┬┴────┬┴────┬┴────┬┴────┬┴────┬┴────┬┴────┬┴────┲┷━━━━━┻━━━━━━┫
┃             │ Z   │ Ž X │ C ¤ │ V   │ B   │ N   │ M   │ ; < │ : > │ ?   ┃             ┃
┃Shift ⇧      │ z   │ ž x │ c © │ v   │ b   │ n   │ m   │ , « │ . » │ / … ┃Shift ⇧      ┃
┣━━━━━━━┳━━━━━┷━┳━━━┷━━━┱─┴─────┴─────┴─────┴─────┴─────┴───┲━┷━━━━━╈━━━━━┻━┳━━━━━━━┳━━━┛
┃       ┃       ┃       ┃ ␣                               ⍽ ┃       ┃       ┃       ┃
┃Ctrl   ┃Meta   ┃Alt    ┃ ␣           Space               ⍽ ┃AltGr ⇮┃Menu   ┃Ctrl   ┃
┗━━━━━━━┻━━━━━━━┻━━━━━━━┹───────────────────────────────────┺━━━━━━━┻━━━━━━━┻━━━━━━━┛
```

Druga rozkladka zasnovana na `us` z dodavannjam ukrajins'kyh literamy z akcentamy. Cja rozkladka klaviš nazyvajet'sja `coder` i pidhodyt' dlja programistiv.

## Vstanovlennja

### Arch/Manjaro Linux

Dlja vstanovlennja z **AUR** vykonajte

```bash
paru -S latynka-kbd
```

abo vykorystovujte vaš uljublenyj pomičnyk z paketom [latynka-kbd][latynka-kbd-aur].

## Vykorystannja

Proekt `latynka-kbd` ne je častynoju [xkeyboard-config][]: vy ne zmožete vykorystaty `localectl`. Ale vy možete vykorystovuvaty `setxkbmap` čy skonnfiguruvaty ce vručnu.

Dejaki pryklady:

### Sway

```
input * {
        xkb_layout "latynka,ua,latynka"
        xkb_variant "coder,unicode,"
        xkb_options "grp:win_space_toggle"
        xkb_model "pc105"
}
```

## Vaš vnesok

Bud' laska pročytajte [Contributing](contributing.md) pro detali procesu podannja nam zapytiv na zminy.

## Istorija zmin

Dyvit'sja [ChangeLog](changelog.md)

## Licenzija

[Apache License v2.0](LICENSE)  
[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg?style=flat)](http://www.apache.org/licenses/LICENSE-2.0.html)

[latynka]: https://cutt.ly/latynka "Українська латинка: усі \"за\" та \"проти\" | Кирилиця чи латиниця | Абетка та розкладка клавіатури"
[latynka-kbd-aur]: https://aur.archlinux.org/packages/latynka-kbd
[xkeyboard-config]: https://github.com/freedesktop/xkeyboard-config "X Keyboard Extension"