
#Imaginal Module

#Parameters

:imaginal-delay  

The imaginal-delay parameter controls how long it takes a request or modification request to the imaginal buffer to complete. It can be set to a non-negative time(in seconds) and defaults to 2.

:vidt

The variable imaginal delay time parameter controls whether the actions of the imaginal buffer take exactly the amount of time specified by :imaginal-delay or if they are randomized with the randomized-time command.

#Buffers

Imaginal buffer

Imaginal-action buffer

#Commands

set-imaginal-free

set-imaginal-error

#Vision module

#Parameters
:auto-attend
:optimize-visual
:scene-change-threshold
:test-feats
:visual-attention-latency

#Buffer

visual-location buffer

visual buffer

#Commands

proc-display
remove-visual-finsts


#Commands- p/define-p

p-name {doc-string} condition* ==> action*

p-name::= a symbol that serves as the name of the production for reference

doc-string::= a string which can be used to document the production

condition::=[buffer-test|query|eval|binding|multiple-value-binding]

action::=[buffer-modification|request|buffer-clearing|modification-request|buffer-overwrite|eval|binding|multiple-value-binding|output|!stop!]

buffer-test::=  =buffer>isa chunk-type slot-test*

query::= ?buffer-name> query-test*

query-test::= {1} queried-item query-value

eval :: =[!eval!][!safe-eval!] form

binding :: =[!bind!][!safe-bind!] variable form

multiple-value-binding :: =!mv--bind! (variable) form

output :: =!output! [output-value] (format-string format-args*)|(output-value*)]
