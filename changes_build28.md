## V0.1 Build 28

Release Date: 2017-03-13

### Changelog

#### Chargecards Feature
While using the GE Registry, all Chargecards available in the GE Registry can be configured (multiple selection), this info being used as an additional filter criteria. Roaming is also supported.

#### Level3 Pins Logic refactored

set level3 (green pin color) only if

a) there is a compatible DC plug available

OR

b) the EV has AC FastCharging Capability and the max power (of all compatible plugs) is over 43kW

#### Bugfix: positive Check-In Comment Header

While showing up the last checkin comment, use the .faultDescription heading when the checkin is not a fault.

#### Misc.

- use the new `open_now` API parameter (see https://github.com/remuslazar/EVPlugFinder/pull/14)
- Resolves https://github.com/remuslazar/EVPlugFinderPublic/issues/52

### Changelog (German)

#### Unterstützung von Ladekarten und Roaming

Es können beliebig viele Ladekarten konfiguriert werden, sodass auch (zusätzlich) alle Ladepunkte 
angezeigt werden, wo ein Laden mit einer der konfigurierten Karten (inkl. Roaming) möglich ist.

Die Ladepunkte, wo ein Laden auch ohne Karte möglich ist werden weiterhin trotzdem angezeigt, 
weil diese immer genutzt werden können.

#### Level3 (grüne Pins) Logik geändert

Level3 Ladestationen (grüne Farbe) werden nur dann angezeigt, wenn der Benutzer auch an der jew. 
Ladestation schnell laden kann. Früher wurden fälschlicherweise auch dann Ladestationen als Level3 
angezeigt (grün), wenn der Benutzer das nicht nutzen konnte (z.B. Leaf-Fahrer und Ladestation 
ohne ChaDeMo jedoch mit einem AC Typ2 43kW Anschluss). Diese werden nun korrekt (im o.g. Fall) 
als Level 2 (orange) angezeigt.

#### Bugfix: Check-In Kommentar als Fehlerbeschreibung

Wenn der letzte Check-in positiv und mit einem Kommentar versehen ist, wurde das als "Fehlerbeschreibung" 
angezeigt.

Die Überschrift lautet nun in solchen Fällen "Check-in Kommentar".

#### Sonstiges

- use the new `open_now` API parameter (see https://github.com/remuslazar/EVPlugFinder/pull/14)
- Resolves https://github.com/remuslazar/EVPlugFinderPublic/issues/52
