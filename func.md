# Funktion määritteleminen

Funktion määrittely alkaa aina avainsanalla `func`. Sitten tulee funktion nimi ja sitten sulut. Aaltosulkuihin tulee mitä funktio tekee.

```Go
func melua() {
    fmt.Println("TÖÖT!")
}
```

Jos funktiosta tulee jotain ulos, sulkujen jälkeen kirjoitetaan _paluuarvon_ [_tyyppi_](tyypit.md). `return`-avainsana lopettaa heti funktion suorituksen. Sen yhteydessä myös annetaan arvot jotka tulevat funktiosta ulos.

```Go
func annaViisi() int {
    return 5
}

func pienempiKuinKolme(luku uint32) bool {
    if luku < 3 {
        return true
    }
    return false
}
```

Sulkujen sisään tulevat nimet ja tyypit argumenteille.

```Go
func tervehdi(nimi string) {
    fmt.Println("Hei,", nimi)
}

func tervehdiKohteliaasti(nimi string) {
    tervehdi("arvoisa " + nimi)
}

func summa(a, b int) int {
    return a + b
}
```

[Vähemmän tärkeää tietoa funktion määrittelemisestä](func2.md)