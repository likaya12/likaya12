<xml xmlns="https://developers.google.com/blockly/xml" is_dbot="true" collection="false">
  <variables>
    <variable id="6o_9Nu#$3m#.?zV=ahjK">Deixar em 8 ou 9</variable>
    <variable id="N5h(uF)6G2cql)h{ZR;h">text</variable>
    <variable id=")-9T~6%gxe29l#C#)qts">text1</variable>
    <variable id="LN}r@t3f(x%mM[7-P|ft">text2</variable>
    <variable id="rUPB[)tUi3we;byHr`7]">5 ou 5 segundos</variable>
    <variable id="RHgF*C%#h{|Ha5u;#5j?">Entrada Inicial</variable>
    <variable id="4+UcGJ_mE@7^Z8-d@JaJ">Número de loss ( Não Alterar )</variable>
    <variable id="kQ+Ke(]*eQpM[qgfd~+g">Contador</variable>
    <variable id="FlX%77!9AMWGEu#,)Nme">Parar com perda de</variable>
    <variable id="(obU$~2J]hr/k0`hgX8/">ENTRADA AO VENCER</variable>
    <variable id="^3d~6DUQ!o8XQTn.XB!c">text3</variable>
    <variable id="a?$LW}C4v+XX:Lc%6-OS">LUCRO DESEJADO</variable>
    <variable id="MgsL8H;~`;r/^Tuh1)y=">Gale</variable>
  </variables>
  <block type="trade_definition" id="|,wpfgCRK_O,JHE[$xte" deletable="false" x="0" y="50">
    <statement name="TRADE_OPTIONS">
      <block type="trade_definition_market" id="dqYC5Hzv(BU~|R.^0oBf" deletable="false" movable="false">
        <field name="MARKET_LIST">synthetic_index</field>
        <field name="SUBMARKET_LIST">random_index</field>
        <field name="SYMBOL_LIST">1HZ100V</field>
        <next>
          <block type="trade_definition_tradetype" id="R%UeAWK76$}y,1vTBL9J" deletable="false" movable="false">
            <field name="TRADETYPECAT_LIST">digits</field>
            <field name="TRADETYPE_LIST">overunder</field>
            <next>
              <block type="trade_definition_contracttype" id="JfVv3q5!6HG+a{Z;UcT~" deletable="false" movable="false">
                <field name="TYPE_LIST">both</field>
                <next>
                  <block type="trade_definition_candleinterval" id="=.C+ze:~jIzo%`@vmpxG" deletable="false" movable="false">
                    <field name="CANDLEINTERVAL_LIST">60</field>
                    <next>
                      <block type="trade_definition_restartbuysell" id="-[*XT*?4Y.x*GF[i_*9?" deletable="false" movable="false">
                        <field name="TIME_MACHINE_ENABLED">FALSE</field>
                        <next>
                          <block type="trade_definition_restartonerror" id="gLmQYbPhRZTP;$NyXRfF" deletable="false" movable="false">
                            <field name="RESTARTONERROR">FALSE</field>
                          </block>
                        </next>
                      </block>
                    </next>
                  </block>
                </next>
              </block>
            </next>
          </block>
        </next>
      </block>
    </statement>
    <statement name="INITIALIZATION">
      <block type="variables_set" id="$*k6w0w?HoW%@WJ[CQ[G">
        <field name="VAR" id="6o_9Nu#$3m#.?zV=ahjK">Deixar em 8 ou 9</field>
        <value name="VALUE">
          <block type="math_number" id="32Y!`!Hso?aG%-1Uy8(b">
            <field name="NUM">9</field>
          </block>
        </value>
        <next>
          <block type="variables_set" id="5#2ZirLJF@(|:)/2$qkw">
            <field name="VAR" id="rUPB[)tUi3we;byHr`7]">5 ou 5 segundos</field>
            <value name="VALUE">
              <block type="math_number" id=":N}6E]-XIDi$;w[B!qq}">
                <field name="NUM">1</field>
              </block>
            </value>
            <next>
              <block type="variables_set" id="gOH1q(Lqj,Kv4+[K|s=-">
                <field name="VAR" id="4+UcGJ_mE@7^Z8-d@JaJ">Número de loss ( Não Alterar )</field>
                <value name="VALUE">
                  <block type="math_number" id="t`]#Z4#DVjSp^{RXbqGP">
                    <field name="NUM">2</field>
                  </block>
                </value>
                <next>
                  <block type="variables_set" id="0!#{3_;P@j;~oXkHmGY|">
                    <field name="VAR" id="FlX%77!9AMWGEu#,)Nme">Parar com perda de</field>
                    <value name="VALUE">
                      <block type="math_number" id="49t$ms:#8*kc6Uer8#](">
                        <field name="NUM">1000</field>
                      </block>
                    </value>
                    <next>
                      <block type="variables_set" id="rY9MYKWTV39sxDv;+kdr">
                        <field name="VAR" id="a?$LW}C4v+XX:Lc%6-OS">LUCRO DESEJADO</field>
                        <value name="VALUE">
                          <block type="math_number" id="4cF?LqK#AJV6Jx.44($6">
                            <field name="NUM">1000</field>
                          </block>
                        </value>
                        <next>
                          <block type="variables_set" id="i,bH`bnP@u(WV|7i!Sz`">
                            <field name="VAR" id="RHgF*C%#h{|Ha5u;#5j?">Entrada Inicial</field>
                            <value name="VALUE">
                              <block type="math_number" id="7B-XT,+7XN#v|1Aa($uz">
                                <field name="NUM">0.35</field>
                              </block>
                            </value>
                            <next>
                              <block type="variables_set" id="IxCR1Na7WMsp2@803{L+">
                                <field name="VAR" id="(obU$~2J]hr/k0`hgX8/">ENTRADA AO VENCER</field>
                                <value name="VALUE">
                                  <block type="math_number" id="JCmZC^lr+W)d!Wm0(~pL">
                                    <field name="NUM">0.35</field>
                                  </block>
                                </value>
                                <next>
                                  <block type="variables_set" id="CpM6_k*o?xE[xaZ[Q@_-">
                                    <field name="VAR" id="MgsL8H;~`;r/^Tuh1)y=">Gale</field>
                                    <value name="VALUE">
                                      <block type="math_number" id="`2(cyquM9#yV^pDqZ`gJ">
                                        <field name="NUM">0.8</field>
                                      </block>
                                    </value>
                                  </block>
                                </next>
                              </block>
                            </next>
                          </block>
                        </next>
                      </block>
                    </next>
                  </block>
                </next>
              </block>
            </next>
          </block>
        </next>
      </block>
    </statement>
    <statement name="SUBMARKET">
      <block type="trade_definition_tradeoptions" id="Kszy$t;dmMnU=/jxC1]D">
        <mutation xmlns="http://www.w3.org/1999/xhtml" has_first_barrier="false" has_second_barrier="false" has_prediction="true"></mutation>
        <field name="DURATIONTYPE_LIST">t</field>
        <value name="DURATION">
          <block type="variables_get" id="7a8:-3ae0d--8A)@0h[z">
            <field name="VAR" id="rUPB[)tUi3we;byHr`7]">5 ou 5 segundos</field>
          </block>
        </value>
        <value name="AMOUNT">
          <block type="variables_get" id="IuC0}Qm@Z=mX]d}3?w(3">
            <field name="VAR" id="RHgF*C%#h{|Ha5u;#5j?">Entrada Inicial</field>
          </block>
        </value>
        <value name="PREDICTION">
          <shadow type="math_number_positive" id="YvP)ix?VIAU)B`Ti,MMQ">
            <field name="NUM">5</field>
          </shadow>
          <block type="variables_get" id="+:eFWwjF^q~1G=PBd)#q">
            <field name="VAR" id="6o_9Nu#$3m#.?zV=ahjK">Deixar em 8 ou 9</field>
          </block>
        </value>
      </block>
    </statement>
  </block>
  <block type="after_purchase" id="tv^t?%1u*:W4IT%pX|zi" collapsed="true" x="898" y="50">
    <statement name="AFTERPURCHASE_STACK">
      <block type="controls_if" id="sJy=W27to^xWtEfx^!In">
        <mutation xmlns="http://www.w3.org/1999/xhtml" else="1"></mutation>
        <value name="IF0">
          <block type="contract_check_result" id="f]tjuq1|sUj(]nr6M7kS">
            <field name="CHECK_RESULT">win</field>
          </block>
        </value>
        <statement name="DO0">
          <block type="text_join" id="0S$z$|5B/gB6]hVHfFNe">
            <field name="VARIABLE" id="N5h(uF)6G2cql)h{ZR;h">text</field>
            <statement name="STACK">
              <block type="text_statement" id="X%Gq.^p$,4upbkB:6uG6">
                <value name="TEXT">
                  <shadow type="text" id="wR[F5j:j}_}AIHKj`/@]">
                    <field name="TEXT"></field>
                  </shadow>
                  <block type="text" id="ofXQ2#?`|+.v^e{h7qwK">
                    <field name="TEXT">Killer market</field>
                  </block>
                </value>
                <next>
                  <block type="text_statement" id="712]i{I(V{L6i9.Wc?T^">
                    <value name="TEXT">
                      <shadow type="text" id="4M~2JZK-6NWn8_tB%Lfz">
                        <field name="TEXT"></field>
                      </shadow>
                      <block type="read_details" id="ntYjAA|;7owvxr2YL!M;">
                        <field name="DETAIL_INDEX">4</field>
                      </block>
                    </value>
                  </block>
                </next>
              </block>
            </statement>
            <next>
              <block type="notify" id=".`1tJfY^10WASKPQ$J_~">
                <field name="NOTIFICATION_TYPE">success</field>
                <field name="NOTIFICATION_SOUND">silent</field>
                <value name="MESSAGE">
                  <block type="variables_get" id="P:a_6!^X|`N-X~g:PrFP">
                    <field name="VAR" id="N5h(uF)6G2cql)h{ZR;h">text</field>
                  </block>
                </value>
                <next>
                  <block type="variables_set" id="$qa*:ge{6Bl[W~fx545#">
                    <field name="VAR" id="RHgF*C%#h{|Ha5u;#5j?">Entrada Inicial</field>
                    <value name="VALUE">
                      <block type="variables_get" id="Gkvu^[]/3G:cW|lCmedw">
                        <field name="VAR" id="(obU$~2J]hr/k0`hgX8/">ENTRADA AO VENCER</field>
                      </block>
                    </value>
                    <next>
                      <block type="variables_set" id="?wi*6(=={p4QrTE?E`2~">
                        <field name="VAR" id="kQ+Ke(]*eQpM[qgfd~+g">Contador</field>
                        <value name="VALUE">
                          <block type="math_number" id="Yq%a{YtZLKX!w;j1RXP?">
                            <field name="NUM">0</field>
                          </block>
                        </value>
                        <next>
                          <block type="variables_set" id="6[t)pQa;ZT2W@-@9v[$u">
                            <field name="VAR" id="6o_9Nu#$3m#.?zV=ahjK">Deixar em 8 ou 9</field>
                            <value name="VALUE">
                              <block type="math_number" id="q2_E,aeD4j$(0ZpBYdbz">
                                <field name="NUM">8</field>
                              </block>
                            </value>
                            <next>
                              <block type="variables_set" id="MQ=0$V5s(xkFcK*yxOA_">
                                <field name="VAR" id="rUPB[)tUi3we;byHr`7]">5 ou 5 segundos</field>
                                <value name="VALUE">
                                  <block type="variables_get" id="ENK7$E3PQkxTYfCWa`QH">
                                    <field name="VAR" id="rUPB[)tUi3we;byHr`7]">5 ou 5 segundos</field>
                                  </block>
                                </value>
                                <next>
                                  <block type="trade_again" id="cw].p*FJWZBupT$eqR!M"></block>
                                </next>
                              </block>
                            </next>
                          </block>
                        </next>
                      </block>
                    </next>
                  </block>
                </next>
              </block>
            </next>
          </block>
        </statement>
        <statement name="ELSE">
          <block type="text_join" id=":4hsJB@ruUmH-fJS,4m0">
            <field name="VARIABLE" id=")-9T~6%gxe29l#C#)qts">text1</field>
            <statement name="STACK">
              <block type="text_statement" id="u9XqKYD#Vai.X-[`,uso">
                <value name="TEXT">
                  <shadow type="text" id="y/YHKw_5m-@Kf^i`(yRS">
                    <field name="TEXT"></field>
                  </shadow>
                  <block type="text" id="MiNQ+-d*C683iU0`o4md">
                    <field name="TEXT">B20 Perda -</field>
                  </block>
                </value>
                <next>
                  <block type="text_statement" id="Do5M]Ky9%Gr{(pV#Cz/5">
                    <value name="TEXT">
                      <shadow type="text" id="vmMsInvTJ-hw~JKi6lWx">
                        <field name="TEXT"></field>
                      </shadow>
                      <block type="math_single" id="?fQk@]behN#[bIF{rF[7">
                        <field name="OP">ABS</field>
                        <value name="NUM">
                          <shadow type="math_number" id="9~o+DI$6c3rP,K3E2x%|">
                            <field name="NUM">9</field>
                          </shadow>
                          <block type="read_details" id="0SbR!Yt]O*F2Cb4A+|lS">
                            <field name="DETAIL_INDEX">4</field>
                          </block>
                        </value>
                      </block>
                    </value>
                  </block>
                </next>
              </block>
            </statement>
            <next>
              <block type="notify" id="F)C~I.3[,jjDu_F;ICpi">
                <field name="NOTIFICATION_TYPE">warn</field>
                <field name="NOTIFICATION_SOUND">silent</field>
                <value name="MESSAGE">
                  <block type="variables_get" id="px#T3t]nmR@pu-!CQe;#">
                    <field name="VAR" id=")-9T~6%gxe29l#C#)qts">text1</field>
                  </block>
                </value>
                <next>
                  <block type="math_change" id="0c)nVxs6Nrk$QLnPk)w:">
                    <field name="VAR" id="kQ+Ke(]*eQpM[qgfd~+g">Contador</field>
                    <value name="DELTA">
                      <shadow type="math_number" id="*qO$Mp_db8_!D8g#XKBP">
                        <field name="NUM">1</field>
                      </shadow>
                    </value>
                    <next>
                      <block type="variables_set" id="2F,Ffs8?a5dKUilg%@i[">
                        <field name="VAR" id="rUPB[)tUi3we;byHr`7]">5 ou 5 segundos</field>
                        <value name="VALUE">
                          <block type="variables_get" id="3FZHSh;f4e.sAFJ1A`}=">
                            <field name="VAR" id="rUPB[)tUi3we;byHr`7]">5 ou 5 segundos</field>
                          </block>
                        </value>
                        <next>
                          <block type="variables_set" id="C?C4r`^,0v,D9e*(h^Iw">
                            <field name="VAR" id="6o_9Nu#$3m#.?zV=ahjK">Deixar em 8 ou 9</field>
                            <value name="VALUE">
                              <block type="math_number" id="Hj6D[]Ga/fY{~w/5@TCh">
                                <field name="NUM">5</field>
                              </block>
                            </value>
                            <next>
                              <block type="controls_if" id="6L?zK,]Qws.xo?*(GemE">
                                <value name="IF0">
                                  <block type="logic_compare" id="P)iuYC-KN0]}(W?=;)H+">
                                    <field name="OP">GTE</field>
                                    <value name="A">
                                      <block type="variables_get" id="BS1Kb/,`O@y}{9Od4rV5">
                                        <field name="VAR" id="kQ+Ke(]*eQpM[qgfd~+g">Contador</field>
                                      </block>
                                    </value>
                                    <value name="B">
                                      <block type="variables_get" id="@L`XIY~OfzFLV?E~`X~Q">
                                        <field name="VAR" id="4+UcGJ_mE@7^Z8-d@JaJ">Número de loss ( Não Alterar )</field>
                                      </block>
                                    </value>
                                  </block>
                                </value>
                                <statement name="DO0">
                                  <block type="math_change" id="R7QtsoT2WFk`*MK0_fy*">
                                    <field name="VAR" id="RHgF*C%#h{|Ha5u;#5j?">Entrada Inicial</field>
                                    <value name="DELTA">
                                      <shadow type="math_number" id="h(2BZh#T.]odF-bqQKcd">
                                        <field name="NUM">5</field>
                                      </shadow>
                                      <block type="math_arithmetic" id="Gl2+IAN)5b!-?RayfW3W">
                                        <field name="OP">MULTIPLY</field>
                                        <value name="A">
                                          <shadow type="math_number" id="3J6xZNy/`wRJZUYz4DLX">
                                            <field name="NUM">5</field>
                                          </shadow>
                                          <block type="math_single" id="Dnw,PYK`H_I-M2voTUTl">
                                            <field name="OP">ABS</field>
                                            <value name="NUM">
                                              <shadow type="math_number" id="F8ts_dw*D9O8R7_^C/Mq">
                                                <field name="NUM">9</field>
                                              </shadow>
                                              <block type="read_details" id="cj527u@:f[5O%EPU/jOk">
                                                <field name="DETAIL_INDEX">4</field>
                                              </block>
                                            </value>
                                          </block>
                                        </value>
                                        <value name="B">
                                          <shadow type="math_number" id=");k~+=ZUM,8V7ovDrIH/">
                                            <field name="NUM">5</field>
                                          </shadow>
                                          <block type="variables_get" id="Z~)63Nf5@3llDqm$7(xT">
                                            <field name="VAR" id="MgsL8H;~`;r/^Tuh1)y=">Gale</field>
                                          </block>
                                        </value>
                                      </block>
                                    </value>
                                  </block>
                                </statement>
                              </block>
                            </next>
                          </block>
                        </next>
                      </block>
                    </next>
                  </block>
                </next>
              </block>
            </next>
          </block>
        </statement>
        <next>
          <block type="text_join" id="fS~U8K1ETkV}kGezbOad">
            <field name="VARIABLE" id="LN}r@t3f(x%mM[7-P|ft">text2</field>
            <statement name="STACK">
              <block
