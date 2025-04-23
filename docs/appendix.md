
## Appendix

This page contains additional information and parameters to fully use the ARCAD Transformer Microservices features.

## Conversion of codes

### Opcodes

The table below outlines the conversion of Operation Codes into Generic Data.

<table>
  <thead>
    <tr>
      <th>Factor 1</th>
      <th>Opcode</th>
      <th>Factor 2</th>
      <th>Result</th>
      <th>Generic Data</th>
      <th>High ind</th>
      <th>Low ind</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td></td>
      <td>ADD</td>
      <td>F2</td>
      <td>R</td>
      <td>*R = *R + F2</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>ADDDUR</td>
      <td>F2</td>
      <td>R</td>
      <td></td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>ALLOC</td>
      <td>F2</td>
      <td>R</td>
      <td></td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>BITOFF</td>
      <td>F2</td>
      <td>R</td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>BITON</td>
      <td>F2</td>
      <td>R</td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>CALL</td>
      <td>F2</td>
      <td>R</td>
      <td></td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>CALLB</td>
      <td>F2</td>
      <td>R</td>
      <td></td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>CAT</td>
      <td>F2</td>
      <td>R</td>
      <td>*R = *R + F2</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>CLEAR</td>
      <td></td>
      <td>R</td>
      <td>CLEAR *R</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>CLEAR</td>
      <td>F2</td>
      <td>R</td>
      <td>CLEAR F2 *R</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>CLOSE</td>
      <td>F2</td>
      <td></td>
      <td>CLOSE F2</td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>DEALLOC</td>
      <td></td>
      <td>R</td>
      <td></td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>DIV</td>
      <td>F2</td>
      <td>R</td>
      <td>*R = *R / F2</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>DO</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>DO</td>
      <td></td>
      <td>R</td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>DO</td>
      <td>F2</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>DO</td>
      <td>F2</td>
      <td>R</td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>ELSE</td>
      <td></td>
      <td></td>
      <td>ELSE</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>END</td>
      <td></td>
      <td></td>
      <td>END</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>ENDCS</td>
      <td></td>
      <td></td>
      <td>ENDCS</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>ENDDO</td>
      <td></td>
      <td></td>
      <td>ENDDO</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>ENDFOR</td>
      <td></td>
      <td></td>
      <td>ENDFOR</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>ENDIF</td>
      <td></td>
      <td></td>
      <td>ENDIF</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>ENDMON</td>
      <td></td>
      <td></td>
      <td>ENDMON</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>ENDSL</td>
      <td></td>
      <td></td>
      <td>ENDSL</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>ENDSR</td>
      <td></td>
      <td></td>
      <td>ENDSR</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>EVAL</td>
      <td>F2</td>
      <td></td>
      <td>F2</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>EXCEPT</td>
      <td>F2</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>EXFMT</td>
      <td>F2</td>
      <td></td>
      <td></td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>EXFMT</td>
      <td>F2</td>
      <td>R</td>
      <td></td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>EXSR</td>
      <td>F2</td>
      <td></td>
      <td>EXSR F2</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>EXTRCT</td>
      <td>F2</td>
      <td>R</td>
      <td></td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>FEOD</td>
      <td>F2</td>
      <td></td>
      <td></td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>FORCE</td>
      <td>F2</td>
      <td></td>
      <td>FORCE F2</td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>FOR</td>
      <td>F2</td>
      <td>R</td>
      <td></td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>IF</td>
      <td>F2</td>
      <td></td>
      <td>IF F2</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>ITER</td>
      <td></td>
      <td></td>
      <td>ITER</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>ITER</td>
      <td>F2</td>
      <td></td>
      <td>ITER F2</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>ITER</td>
      <td></td>
      <td>R</td>
      <td>ITER *R</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>ITER</td>
      <td>F2</td>
      <td>R</td>
      <td>ITER F2 *R</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>LEAVE</td>
      <td></td>
      <td></td>
      <td>LEAVE</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>LEAVESR</td>
      <td></td>
      <td></td>
      <td>LEAVESR</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>LOOKUP</td>
      <td>F2</td>
      <td>R</td>
      <td></td>
      <td>%FOUND</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>MOVE</td>
      <td>F2</td>
      <td>R</td>
      <td>MOVE F2 *R</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>MOVEL</td>
      <td>F2</td>
      <td>R</td>
      <td>MOVEL F2 *R</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>MULT</td>
      <td>F2</td>
      <td>R</td>
      <td>*R = *R * F2</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>OPEN</td>
      <td>F2</td>
      <td></td>
      <td>OPEN F2</td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>POST</td>
      <td>F2</td>
      <td></td>
      <td>POST F2</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>READ</td>
      <td>F2</td>
      <td></td>
      <td></td>
      <td>%EOF</td>
      <td>%ERROR</td>
    </tr>
    <tr>
      <td></td>
      <td>READC</td>
      <td>F2</td>
      <td></td>
      <td></td>
      <td>%EOF</td>
      <td>%ERROR</td>
    </tr>
    <tr>
      <td></td>
      <td>READE</td>
      <td>F2</td>
      <td></td>
      <td></td>
      <td>%EOF</td>
      <td>%ERROR</td>
    </tr>
    <tr>
      <td></td>
      <td>READP</td>
      <td>F2</td>
      <td></td>
      <td></td>
      <td>%EOF</td>
      <td>%ERROR</td>
    </tr>
    <tr>
      <td></td>
      <td>READPE</td>
      <td>F2</td>
      <td></td>
      <td></td>
      <td>%EOF</td>
      <td>%ERROR</td>
    </tr>
    <tr>
      <td></td>
      <td>REALLOC</td>
      <td>F2</td>
      <td>R</td>
      <td></td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>REL</td>
      <td></td>
      <td>R</td>
      <td></td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>RETURN</td>
      <td></td>
      <td></td>
      <td>RETURN</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>SELECT</td>
      <td></td>
      <td></td>
      <td>SELECT</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>SEND</td>
      <td>F2</td>
      <td></td>
      <td>SEND F2</td>
      <td>%ERROR</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>SETON</td>
      <td>F2</td>
      <td></td>
      <td>SETON F2</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>SHTDN</td>
      <td>F2</td>
      <td></td>
      <td>SHTDN F2</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>SUB</td>
      <td>F2</td>
      <td>R</td>
      <td>*R = *R - F2</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>TAG</td>
      <td></td>
      <td></td>
      <td>TAG</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>WHEN</td>
      <td>F2</td>
      <td></td>
      <td>WHEN F2</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>WRITE</td>
      <td>F2</td>
      <td></td>
      <td></td>
      <td>%ERROR</td>
      <td></td>
    </tr>
  </tbody>
</table>

### Fix and Free Opcodes

The tables below outline the conversion of Operation Codes into Generic Ppcodes.

   | Fix and Free |  Original Opcode    | Generic Opcode |
   |--------------|---------------------|----------------|
   | FIX   | ACQ    | ACQUIRE |
   | FREE  | ACQ    | ACQUIRE |
   | FIX   | ADD    | ASSIGN  |
   | FIX   | ADDDUR | DURATION |
   | FIX   | ALLOC  | STORAGE |
   | FIX   | AND    | LOGICAND |
   | FIX   | BEGSR  | STARTSR |
   | FREE  | BEGSR  | STARTSR |
   | FIX   | BITOFF | BITOFF  |
   | FIX   | BITON  | BITON   |
   | FIX   | CAB    | GOTO    |
   | FIX   | CALL   | CALL    |
   | FIX   | CALLB  | CALL    |
   | FIX   | CALLP  | CALL    |
   | FREE  | CALLP  | CALL    |
   | FIX   | CAS    | EXSR    |
   | FIX   | CAT    | CONCAT  |
   | FIX   | CHAIN  | SEARCH  |
   | FREE  | CHAIN  | SEARCH  |
   | FIX   | CHECK  | SEARCH  |
   | FIX   | CHECKR | SEARCHR |
   | FIX   | CLEAR  | CLEAR   |
   | FREE  | CLEAR  | CLEAR   |
   | FIX   | CLOSE  | CLOSE   |
   | FREE  | CLOSE  | CLOSE   |
   | FIX   | COMMIT | COMMIT  |
   | FREE  | COMMIT | COMMIT  |
   | FIX   | COMP   | EQUAL   |
   | FIX   | DATA-GEN | DATA-GEN |
   | FREE  | DATA-GEN | DATA-GEN |
   | FIX   | DATA-INTO | DATA-INTO |
   | FREE  | DATA-INTO | DATA-INTO |
   | FIX   | DEALLOC | STORAGE |
   | FREE  | DEALLOC | STORAGE |
   | FIX   | DELETE | DELETE  |
   | FREE  | DELETE | DELETE  |
   | FIX   | DIV    | ASSIGN  |
   | FIX   | DO     | GROUP   |
   | FIX   | DOU    | GROUP   |
   | FREE  | DOU    | GROUP   |
   | FIX   | DOUEQ  | DOU     |
   | FIX   | DOUGE  | DOU     |
   | FIX   | DOUGT  | DOU     |
   | FIX   | DOULE  | DOU     |
   | FIX   | DOULT  | DOU     |
   | FIX   | DOUNE  | DOU     |
   | FIX   | DOW    | GROUP   |
   | FREE  | DOW    | GROUP   |
   | FIX   | DOWEQ  | DOW     |
   | FIX   | DOWGE  | DOW     |
   | FIX   | DOWGT  | DOW     |
   | FIX   | DOWLE  | DOW     |
   | FIX   | DOWLT  | DOW     |
   | FIX   | DOWNE  | DOW     |
   | FIX   | DSPLY  | DISPLAY |
   | FREE  | DSPLY  | DISPLAY |
   | FIX   | DUMP   | DUMP    |
   | FREE  | DUMP   | DUMP    |
   | FIX   | ELSE   | ELSE    |
   | FREE  | ELSE   | ELSE    |
   | FIX   | ELSEIF | ELSEIF  |
   | FREE  | ELSEIF | ELSEIF  |
   | FIX   | END    | ENDGROUP |
   | FIX   | ENDCS  | ENDGROUP |
   | FIX   | ENDDO  | ENDGROUP |
   | FREE  | ENDDO  | ENDGROUP |
   | FIX   | ENDFOR | ENDGROUP |
   | FREE  | ENDFOR | ENDGROUP |
   | FIX   | ENDIF  | ENDIF   |
   | FREE  | ENDIF  | ENDGROUP |
   | FIX   | ENDMON | ENDGROUP |
   | FREE  | ENDMON | GROUP   |
   | FIX   | ENDSL  | ENDGROUP |
   | FREE  | ENDSL  | ENDGROUP |
   | FIX   | ENDSR  | ENDSR   |
   | FREE  | ENDSR  | ENDSR   |
   | FIX   | EVAL   | ASSIGN  |
   | FREE  | EVAL   | ASSIGN  |
   | FIX   | EVAL-CORR | ASSIGN  |
   | FREE  | EVAL-CORR | ASSIGN  |
   | FIX   | EVALR  | ASSIGN  |
   | FREE  | EVALR  | ASSIGN  |
   | FIX   | EXCEPT | INSERT  |
   | FREE  | EXCEPT | INSERT  |
   | FIX   | EXFMT  | DISPLAY |
   | FREE  | EXFMT  | DISPLAY |
   | FIX   | EXSR   | CALLSR  |
   | FREE  | EXSR   | CALLSR  |
   | FIX   | EXTRCT | EXTRACT |
   | FIX   | FOR    | GROUP   |
   | FREE  | FOR    | GROUP   |
   | FREE  | FOR-EACH | GROUP |
   | FIX   | GOTO   | GOTO    |
   | FIX   | IF     | IF      |
   | FREE  | IF     | IF      |
   | FIX   | IFEQ   | IF      |
   | FIX   | IFGE   | IF      |
   | FIX   | IFLE   | IF      |
   | FIX   | IFNE   | IF      |
   | FIX   | IN     | ASSIGN  |
   | FREE  | IN     | ASSIGN  |
   | FIX   | ITER   | GROUP   |
   | FREE  | ITER   | GROUP   |
   | FIX   | KFLD   |         |
   | FIX   | KLIST  |         |
   | FIX   | LEAVE  | GROUP   |
   | FREE  | LEAVE  | GROUP   |
   | FIX   | LEAVESR | GROUP  |
   | FREE  | LEAVESR | GROUP  |
   | FIX   | LOOKUP | SEARCH  |
   | FIX   | MHHZO  | ASSIGN  |
   | FIX   | MHLZO  | ASSIGN  |
   | FIX   | MLHZO  | ASSIGN  |
   | FIX   | MLLZO  | ASSIGN  |
   | FIX   | MONITOR | GROUP  |
   | FIX   | MOVE   | ASSIGNR |
   | FIX   | MOVEA  | ASSIGNA |
   | FIX   | MOVEL  | ASSIGN  |
   | FIX   | MULT   | ASSIGN  |
   | FIX   | MVR    | ASSIGN  |
   | FIX   | OCCUR  | OCCUR   |
   | FIX   | ON-ERROR | GROUP |
   | FREE  | ON-ERROR | GROUP |
   | FIX   | ON-EXIT | GROUP  |
   | FREE  | ON-EXIT | GROUP  |
   | FIX   | OPEN   | OPEN    |
   | FREE  | OPEN   | OPEN    |
   | FIX   | OR     | LOGICOR |
   | FIX   | OTHER  | GROUP   |
   | FREE  | OTHER  | GROUP   |
   | FIX   | OUT    | ASSIGN  |
   | FREE  | OUT    | ASSIGN  |
   | FIX   | PLIST  | PLIST   |
   | FIX   | POST   | POST    |
   | FREE  | POST   | POST    |
   | FIX   | READ   | RECORD  |
   | FREE  | READ   | RECORD  |
   | FIX   | READC  | RECORD  |
   | FREE  | READC  | RECORD  |
   | FIX   | READE  | RECORD  |
   | FREE  | READE  | RECORD  |
   | FIX   | READP  | RECORD  |
   | FREE  | READP  | RECORD  |
   | FIX   | READPE | RECORD  |
   | FREE  | READPE | RECORD  |
   | FIX   | REALLOC | STORAGE|
   | FIX   | REL    | RELEASE |
   | FREE  | REL    | RELEASE |
   | FIX   | RESET  | RESET   |
   | FREE  | RESET  | RESET   |
   | FIX   | RETURN | RETURN  |
   | FREE  | RETURN | RETURN  |
   | FIX   | ROLBK  | REVOKE  |
   | FREE  | ROLBK  | REVOKE  |
   | FIX   | SCAN   | SEARCH  |
   | FIX   | SELECT | GROUP   |
   | FREE  | SELECT | GROUP   |
   | FIX   | SETGT  | LIMIT   |
   | FREE  | SETGT  | LIMIT   |
   | FIX   | SETLL  | LIMIT   |
   | FREE  | SETLL  | LIMIT   |
     