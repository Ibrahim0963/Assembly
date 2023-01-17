Assembly Sprache ist eine niedrigste Ebene Programmiersprache, die direkt auf die Hardware-Befehle des Computers zugreift. Sie ermöglicht es dem Programmierer, direkt auf die Register und Speicherzellen des Prozessors zuzugreifen und Befehle auszuführen. Assembly Sprache erfordert jedoch ein tiefes Verständnis der Hardware-Architektur des Computers und ist daher in der Regel schwieriger zu lernen und zu verwenden als höhere Ebene Sprachen wie C oder Java. Es wird hauptsächlich in der System- und Embedded-Programmierung eingesetzt, da es eine sehr gute Kontrolle über die Hardware ermöglicht.

In Assembly Sprache gibt es keine Variablen wie in höheren Ebene Sprachen, stattdessen muss der Programmierer direkt auf die Speicherzellen zugreifen, um Daten zu speichern und zu manipulieren. Es gibt auch keine Schleifen oder Verzweigungen wie in höheren Ebene Sprachen, stattdessen muss der Programmierer Befehle verwenden, um den Programmfluss zu steuern.

Es gibt auch viele verschiedene Assembly Sprachen, da jeder Prozessor eine andere Architektur hat und daher eine andere Assembly Sprache verwendet werden muss. Beispiele für Assembly Sprachen sind x86 Assembly für Intel-Prozessoren und ARM Assembly für ARM-Prozessoren.

Ein Beispiel für Assembly Code könnte sein:
```
MOV AX, 5
MOV BX, AX
ADD BX, 3
MOV CX, BX
```
Dieser Code bewegt den Wert 5 in das Register AX, dann bewegt den Inhalt von AX in BX und fügt 3 hinzu, schließlich bewegt der Wert in BX in CX Register.

Die Assembly Sprache bietet einige Vorteile gegenüber höheren Ebene Sprachen:

1.  Hohe Leistung: Da Assembly Sprache direkt auf die Hardware-Befehle des Computers zugreift, kann es sehr effizient und schnell ausgeführt werden. Es ermöglicht es dem Programmierer, die Leistung des Codes sehr genau zu steuern und zu optimieren.
    
2.  Kontrolle über die Hardware: Assembly Sprache ermöglicht es dem Programmierer, direkt auf die Register und Speicherzellen des Prozessors zuzugreifen und Befehle auszuführen. Dies ermöglicht eine sehr gute Kontrolle über die Hardware und ermöglicht es, spezielle Funktionen oder Hardware-Eigenschaften zu nutzen, die in höheren Ebene Sprachen nicht verfügbar sind.
    
3.  Einfache Fehlerdiagnose: Da Assembly Sprache direkt auf die Hardware-Befehle des Computers zugreift, kann es einfacher sein, Fehler im Code zu diagnostizieren und zu beheben, da es weniger Abstraktionsebenen gibt.
    
4.  Embedded-Systeme: Assembly Sprache wird oft in Embedded-Systemen verwendet, da es eine sehr gute Kontrolle über die Hardware ermöglicht und es ermöglicht, sehr kompakten und effizienten Code zu erstellen, der auf begrenztem Speicherplatz ausgeführt werden kann.
    
5.  Systemprogrammierung: Assembly Sprache wird oft in der Systemprogrammierung verwendet, da es eine sehr gute Kontrolle über die Hardware ermöglicht und es ermöglicht, sehr effizienten und schnellen Code zu erstellen, der auf niedriger Ebene ausgeführt werden kann.


## Data-Size
Die Data-Size, die ein Prozessor unterstützt, hängt von der Architektur des Prozessors ab. Einige Prozessoren unterstützen nur 8-Bit-Daten (ein Byte), während andere Prozessoren 32-Bit- oder 64-Bit-Daten unterstützen können.

Ein Beispiel ist der Intel x86-Prozessor, der 8-Bit, 16-Bit, 32-Bit und 64-Bit-Daten unterstützt. Dies bedeutet, dass der Prozessor Befehle ausführen kann, die auf 8-Bit-Werte (1 Byte), 16-Bit-Werte (2 Bytes), 32-Bit-Werte (4 Bytes) und 64-Bit-Werte (8 Bytes) zugreifen.

Andere Beispiele sind der ARM Cortex-Prozessor, der 32-Bit-Daten unterstützt und der PowerPC-Prozessor, der 32-Bit und 64-Bit-Daten unterstützt.

## Register
Registrierungen sind in der Regel in verschiedene Typen unterteilt, z.B. Arithmetik- und Logikregister (ALU), Steuerregister, Adressregister und Datenregister. Jeder Typ von Register hat seine eigene spezifische Funktion und wird verwendet, um bestimmte Arten von Operationen auszuführen.

Ein Beispiel für ein Register in der Assembly Sprache ist das AX-Register, das in der x86-Architektur verwendet wird. Es kann verwendet werden, um Daten zu speichern und zu manipulieren und wird oft in arithmetischen und logischen Operationen verwendet.

Ein anderes Beispiel ist das PC-Register (Program Counter) in der ARM-Architektur, das verwendet wird, um den aktuellen Ausführungspunkt im Code zu speichern.


## Prozessor
Der Prozessor steuert die Ausführung von Anweisungen durch den fetch-decode-execute Zyklus oder den Ausführungszyklus. Dieser besteht aus drei aufeinanderfolgenden Schritten: dem Abrufen der Anweisung aus dem Speicher, dem Dekodieren oder Identifizieren der Anweisung und dem Ausführen der Anweisung.

Der Prozessor kann ein oder mehrere Bytes Speicher auf einmal zugreifen. Wenn er eine hexadezimale Zahl wie 0725H aus dem Speicher lädt, benötigt diese Zahl zwei Bytes Speicher. Das High-Order-Byte oder das meist signifikante Byte ist 07 und das Low-Order-Byte ist 25.

Der Prozessor speichert Daten in umgekehrter Byte-Reihenfolge, d.h. ein Low-Order-Byte wird in einer niedrigen Speicheradresse gespeichert und ein High-Order-Byte in einer hohen Speicheradresse. Wenn der Prozessor also den Wert 0725H aus dem Register in den Speicher überträgt, wird zuerst 25 in die niedrigere Speicheradresse und 07 in die nächste Speicheradresse übertragen.

Der Prozessor kann auch auf Daten im Speicher mit Absolute-Adressen oder Segment-Adressen (mit Offset-Wert) zugreifen. Absolute Adressen sind direkte Verweise auf eine bestimmte Speicherstelle, während Segment-Adressen den Startpunkt eines Speichersegments mit einem Offset-Wert angeben.


## Assembly-Programm
Ein Assembly-Programm kann in drei Abschnitte unterteilt werden:

1.  data section
2.  bss section
3.  text section (abschnitt)

Der data section wird verwendet, um initialisierte Daten oder Konstanten zu deklarieren. Diese Daten ändern sich während der Laufzeit nicht. Sie können verschiedene konstante Werte, Dateinamen oder Puffergroßen usw. in diesem Abschnitt deklarieren.

Der bss section wird verwendet, um Variablen zu deklarieren.

Der text section wird verwendet, um den tatsächlichen Code zu speichern. Dieser Abschnitt muss mit der globalen Deklaration _start beginnen, die dem Kernel sagt, wo die Programmausführung beginnt.

## Segmentiertes Speichermodell
Ein segmentiertes Speichermodell teilt den Systemspeicher in Gruppen von unabhängigen Segmenten auf, die von Zeigern in den Segmentregistern referenziert werden. Jedes Segment wird verwendet, um einen bestimmten Datentyp zu enthalten. Ein Segment wird verwendet, um Anweisungscodes zu enthalten, ein anderes Segment speichert die Datenelemente und ein drittes Segment behält den Programmstack.

Data-Segment: Es wird durch den .data-Abschnitt und den .bss-Abschnitt repräsentiert. Der .data-Abschnitt wird verwendet, um den Speicherbereich zu deklarieren, in dem die Datenelemente für das Programm gespeichert werden. Dieser Abschnitt kann nach der Deklaration der Datenelemente nicht erweitert werden und bleibt während des gesamten Programms statisch.

Der .bss-Abschnitt ist ebenfalls ein statischer Speicherabschnitt, der Puffer für später im Programm zu deklarierende Daten enthält. Dieser Pufferspeicher ist mit Nullen gefüllt.

Code-Segment: Es wird durch den .text-Abschnitt repräsentiert. Dieser definiert einen Bereich im Speicher, der die Anweisungscodes speichert. Dies ist ebenfalls ein festes Gebiet.

Stack: Dieses Segment enthält Datenwerte, die an Funktionen und Prozeduren innerhalb des Programms übergeben werden.

## Prozessorregister
Der Prozessor führt hauptsächlich Datenverarbeitungen durch. Diese Daten können im Speicher gespeichert und von dort aus aufgerufen werden. Das Lesen von Daten aus und das Speichern von Daten in den Speicher verlangsamt jedoch den Prozessor, da es komplexe Prozesse des Sendens der Datenanforderung über den Steuerbus und in die Speichereinheit sowie des Empfangens der Daten über denselben Kanal beinhaltet.

Um die Prozessorvorgänge zu beschleunigen, enthält der Prozessor einige interne Speicherstandorte, die als Register bezeichnet werden.

Die Register speichern Datenelemente für die Verarbeitung, ohne auf den Speicher zugreifen zu müssen. In den Prozessorchip sind eine begrenzte Anzahl von Registern integriert.

Prozessorregister Es gibt zehn 32-Bit- und sechs 16-Bit-Prozessorregister in der IA-32-Architektur. Die Register werden in drei Kategorien unterteilt:
- Allgemeine Register
- Steuerregister
- Segmentregister.

Die allgemeinen Register werden weiter in folgende Gruppen unterteilt:
- Datenregister
- Zeigerregister
- Indexregister.

## Datenregister
Die Datenregister werden für arithmetische, logische und andere Operationen verwendet. Diese 32-Bit-Register können auf drei Arten verwendet werden:
- Als vollständige 32-Bit-Datenregister: EAX, EBX, ECX, EDX.
  - Die unteren Hälften der 32-Bit-Register können als vier 16-Bit-Datenregister verwendet werden: AX, BX, CX und DX.
	  - Die unteren und oberen Hälften der oben genannten vier 16-Bit-Register können als acht 8-Bit-Datenregister verwendet werden: AH, AL, BH, BL, CH, CL, DH und DL.

![image](https://user-images.githubusercontent.com/48016716/212926678-8f274c7a-2cca-426c-8992-c09d10d73ab0.png)

Einige dieser Datenregister haben eine spezielle Verwendung in arithmetischen Operationen.

**AX** ist der primäre Akkumulator; es wird in Ein-/Ausgabe- und den meisten arithmetischen Anweisungen verwendet. Zum Beispiel wird bei einer Multiplikationsoperation ein Operand im EAX-, AX- oder AL-Register gemäß der Größe des Operanden gespeichert.

**BX** wird als Basisregister bezeichnet, da es in indexierten Adressierungen verwendet werden kann.

**CX** wird als Zählerregister bezeichnet, da die ECX-, CX-Register die Schleifenanzahl in iterativen Operationen speichern.

**DX** wird als Datenregister bezeichnet. Es wird auch in Ein-/Ausgabe-Operationen verwendet. Es wird auch zusammen mit AX-Register und DX für Multiplikations- und Divisionen mit großen Werten verwendet.

## Pointer-Register
Die Pointer-Register sind 32-Bit-EIP-, ESP- und EBP-Register sowie die entsprechenden 16-Bit-rechten Teile IP, SP und BP. Es gibt drei Kategorien von Pointer-Registern:

**Instruction Pointer (IP)** - Das 16-Bit-IP-Register speichert die Offset-Adresse der nächsten auszuführenden Anweisung. IP in Verbindung mit dem CS-Register (als CS: IP) gibt die vollständige Adresse der aktuellen Anweisung im Codesegment an.

**Stack Pointer (SP)** - Das 16-Bit-SP-Register stellt den Offset-Wert innerhalb des Programmstapels bereit. SP in Verbindung mit dem SS-Register (SS: SP) bezieht sich auf die aktuelle Position von Daten oder Adressen innerhalb des Programmstapels.

**Base Pointer (BP)** - Das 16-Bit-BP-Register hilft hauptsächlich beim Referenzieren der an eine Unterroutine übergebenen Parametervariablen. Die Adresse im SS-Register wird mit dem Offset in BP kombiniert, um den Speicherort des Parameters zu erhalten. BP kann auch zusammen mit DI und SI als Basisregister für spezielle Adressierung verwendet werden.

![image](https://user-images.githubusercontent.com/48016716/212927075-f465e4fb-c0a1-4d44-a530-ecfbed6f19e7.png)

## Index-Register
Die 32-Bit-Index-Register ESI und EDI und ihre 16-Bit-rechten Teile SI und DI werden für indexierte Adressierung verwendet und manchmal in Addition und Subtraktion verwendet. Es gibt zwei Sets von Indexzeigern:

**Source Index (SI)** - Es wird als Quellindex für String-Operationen verwendet.

**Destination Index (DI)** - Es wird als Zielindex für String-Operationen verwendet. Die Index-Register werden verwendet, um die Position von Daten im Speicher in Bezug auf einen bestimmten Index oder Offset zu verfolgen. Sie ermöglichen es dem Prozessor, Daten schneller und effizienter aus dem Speicher zu lesen und zu schreiben, indem sie die Adresse des Datensatzes im Speicher angeben.

![image](https://user-images.githubusercontent.com/48016716/212927227-8e04248c-974c-445f-ad4f-fd209157ee83.png)

## Instruktionszeiger-Register
Viele Anweisungen beinhalten Vergleiche und mathematische Berechnungen und ändern den Status der Flags und einige andere bedingte Anweisungen testen den Wert dieser Status-Flags, um den Ablaufsteuerung an einen anderen Ort zu übertragen.

Die häufigsten Flags sind:

Overflow Flag (OF) - Es gibt an, ob ein Überlauf eines höherwertigen Bits (linkes Bit) nach einer signed Arithmetikoperation auftritt.

Direction Flag (DF) - Es bestimmt die Richtung nach links oder rechts für das Verschieben oder Vergleichen von Stringdaten. Wenn der Wert von DF 0 ist, erfolgt die Stringoperation von links nach rechts und wenn der Wert auf 1 gesetzt ist, erfolgt die Stringoperation von rechts nach links.

Interrupt Flag (IF) - Es bestimmt, ob externe Unterbrechungen wie Tastatureingaben usw. ignoriert oder verarbeitet werden sollen. Es deaktiviert die externe Unterbrechung, wenn der Wert 0 ist und aktiviert Unterbrechungen, wenn auf 1 gesetzt.

Trap Flag (TF) - Es ermöglicht die Einstellung des Prozessors im Einzelschrittmodus. Das DEBUG-Programm, das wir verwendet haben, setzt das Trap-Flag, so dass wir die Ausführung schrittweise durchlaufen können.

Sign Flag (SF) - Es zeigt das Vorzeichen des Ergebnisses einer arithmetischen Operation an. Dieser Flag wird entsprechend dem Vorzeichen eines Datenelements nach der arithmetischen Operation gesetzt. Das Vorzeichen wird durch das höherwertige, linkeste Bit angezeigt. Ein positives Ergebnis setzt den Wert von SF auf 0 zurück und ein negatives Ergebnis setzt es auf 1.

Zero Flag (ZF) - Es zeigt das Ergebnis einer arithmetischen oder Vergleichsoperation an. Ein nicht-null Ergebnis setzt den Null-Flag auf 0 zurück und ein Null-Ergebnis setzt es auf 1.

Auxiliary Carry Flag (AF) - verwendet für spezialisierte Arithmetik. Der AF wird gesetzt, wenn eine 1-Byte-Arithmetikoperation einen Carry von Bit 3 in Bit 4 verursacht.

Parity Flag (PF) - Es gibt an, wie viele 1-Bits im Ergebnis einer arithmetischen Operation enthalten sind. Eine gerade Anzahl von 1-Bits setzt den Paritätsflag auf 0 zurück und eine ungerade Anzahl von 1-Bits setzt ihn auf 1.

Carry Flag (CF) - Es enthält den Carry von 0 oder 1 von einem höherwertigen Bit (linkes Bit) nach einer arithmetischen Operation. Es speichert auch den Inhalt des letzten Bits einer Verschiebe- oder Rotationsoperation.


In der Assembly-Programmierung benötigt ein Programm Zugriff auf Speicherpositionen. Alle Speicherpositionen innerhalb eines Segments sind relativ zur Startadresse des Segments. Ein Segment beginnt in einer Adresse, die durch 16 oder hexadezimal 10 teilbar ist. Daher ist die rechteste Hex-Ziffer in allen solchen Speicheradressen 0, die normalerweise nicht in den Segmentregistern gespeichert wird.

Die Segmentregister speichern die Startadressen eines Segments. Um die genaue Position von Daten oder Anweisungen innerhalb eines Segments zu erhalten, wird ein Offsetwert (oder Versatz) benötigt. Um auf eine beliebige Speicherposition in einem Segment zu verweisen, kombiniert der Prozessor die Segmentadresse im Segmentregister mit dem Offsetwert der Position.

## Linux System Calls
Es gibt viele verschiedene Systemaufrufe, die von einem Programm verwendet werden können, um bestimmte Aktionen auszuführen, wie z.B. das Lesen und Schreiben von Dateien, das Anlegen von Prozessen und das Verwalten von Netzwerkverbindungen. In Linux können diese Systemaufrufe über Interrupts an den Kernel übermittelt werden.

Um einen Systemaufruf in einem Assembly-Programm auszuführen, müssen Sie die Nummer des gewünschten Aufrufs in den EAX-Register legen, die Argumente für den Aufruf in den EBX, ECX usw. Register speichern und den entsprechenden Interrupt (80h) aufrufen. Das Ergebnis wird normalerweise im EAX-Register zurückgegeben.

Es gibt sechs Register, die die Argumente des verwendeten Systemaufrufs speichern. Dies sind die EBX, ECX, EDX, ESI, EDI und EBP. Diese Register nehmen die aufeinanderfolgenden Argumente auf, beginnend mit dem EBX-Register. Wenn es mehr als sechs Argumente gibt, wird die Speicheradresse des ersten Arguments im EBX-Register gespeichert.


![image](https://user-images.githubusercontent.com/48016716/212938620-df28be90-d8fa-49e5-9d5f-a613bd8593d5.png)













