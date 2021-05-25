# pumltools

(work in progress)

#### Convert generated Sequence Diagrams to Communication Diagrams

```
puml_fd_cat |
    ack --match '-> "?(MyClassA|MyClassB)"' |
    ack -v "RSpec|initialize" |
    puml_communication |
    puml_uml_wrap |
    cat > "communication.puml"
```

#### Convert generated Sequence Diagrams to References Diagram

```
puml_fd_cat |
    ack --match '-> "?(MyClassA|MyClassB)"' |
    ack -v "RSpec|initialize" |
    puml_references |
    puml_uml_wrap |
    cat > "references.puml"
```
