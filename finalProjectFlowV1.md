```mermaid
    flowchart TB
    Start([Wait for time to be input])

    ST1(Wait for submit to be pressed)

    ST2(Make a loop with # sec itterations)

    ST3(Make i variable = to # of secs)

    Start --> ST1 --> ST2 --> ST3 --> Dec1

    Dec1{i == 0}
    D1y(Counter finished)
    D1n(Print i)
    D1n2(i--)
    D1n3(delay 1 sec)
    Dec1 -->|Yes| D1y --> D1y2 --> End
    Dec1 -->|No| D1n --> D1n2 --> D1n3--> Dec1
    D1y2(Play sound)

    End([Pause buzzer and wait for new submission])