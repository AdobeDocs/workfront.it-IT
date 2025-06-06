---
title: Panoramica sulla versione del terzo trimestre 2024
description: Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del terzo trimestre 2024. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 0%

---

# Panoramica sulla versione del terzo trimestre 2024

Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del terzo trimestre 2024. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.

Il webinar sulla versione live 24.7 è stato annullato, ma puoi ancora [guardare una dimostrazione video delle funzionalità 24.7 qui](https://video.tv.adobe.com/v/3430532/%20).

<span class="preview">Le funzioni fuori ciclo (quelle rilasciate in produzione prima della data di rilascio del terzo trimestre 2024) sono evidenziate in giallo.</span>

>[!IMPORTANT]
>
>La versione 23.3 includeva l’opzione per spostare l’organizzazione alle versioni mensili. Pertanto, Workfront ha modificato lo schema di numerazione delle versioni per tenere conto delle versioni mensili e trimestrali. Il primo numero indica l’anno e il secondo il mese del rilascio. Esempio: la versione di aprile 2024 è la 24.4.
>
>Salvo diversa indicazione, i rilasci mensili e trimestrali dovrebbero essere disponibili il giovedì della seconda settimana completa del mese.
>
>| Versione mensile | Versione trimestrale |
>|----|----|
>| <ul><li>24.5 (16 maggio 2024)</li><li>24.6 (13 giugno 2024)</li><li>24.7 (18 luglio 2024)</li></ul> | <ul><li>24.7 (18 luglio 2024)</li></ul> |
>
>Per ulteriori informazioni sul processo di rilascio rapido, vedere [Attivare o disattivare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Miglioramenti di Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Miglioramenti alla gestione finanziaria](#financial-management-enhancements)
* [Miglioramenti dell’integrazione](#integration-enhancements)
* [Miglioramenti al progetto](#project-enhancements)
* [Miglioramenti delle bozze](#proofing-enhancements)
* [Miglioramenti alla gestione delle risorse](#resource-management-enhancements)
* [Altri miglioramenti](#other-enhancements)

### Miglioramenti per gli amministratori

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Funzionalità</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Date di rilascio</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Le regole business sono ora disponibili</a></p>
                        [!BADGE In produzione &#x200B;]{type=Informative}
                        <p>Gli amministratori possono ora aggiungere regole business nell’area Configurazione di Workfront.</p>
                        <p>Una regola business consente di applicare la convalida agli oggetti di Workfront e di impedire agli utenti di creare, modificare o eliminare un oggetto quando vengono soddisfatte determinate condizioni. Le regole vengono create utilizzando una formula simile ai campi calcolati nei moduli personalizzati.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 4 luglio 2024</p>
                            </li>
                            <li>
                                <p>Versione di produzione per tutti i clienti: con la versione 24.7 (18 luglio 2024)</p>
                            </li>
                        </ul>
                        <p><i>Disponibile solo per le organizzazioni che fanno parte del nuovo piano Ultimate.</i></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">La finestra di progettazione dei moduli personalizzati è disponibile in Adobe Workfront</a></p>
                        [!BADGE In produzione &#x200B;]{type=Informative}
                        <p>Con la versione 24.7, il progettista di moduli sarà generalmente disponibile e diventerà l’esperienza predefinita per la creazione e la modifica di moduli personalizzati in Adobe Workfront. Quando si crea un nuovo modulo personalizzato o si apre un modulo esistente, viene visualizzata l'area di lavoro in stile area di lavoro del progettista del modulo.</p>
                        <p>Dopo questa versione, non sarà più possibile tornare al generatore di moduli legacy.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 19 giugno 2024</p>
                            </li>
                            <li>
                                <p>Versione di produzione per tutti i clienti: con la versione 24.7 (18 luglio 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Spostamento di oggetti tra ambienti Workfront con promozione dell'ambiente</a></p>
                        [!BADGE In produzione &#x200B;]{type=Informative}
                        <p>La promozione dell’ambiente consente di spostare gli oggetti da un ambiente Workfront a un altro, ad esempio da un ambiente sandbox a un ambiente di produzione. È possibile configurare e testare gli oggetti senza alcun rischio per i dati e i record dell'organizzazione. È quindi possibile spostare tali oggetti in produzione senza doverli riconfigurare, risparmiando tempo e fatica.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di produzione per tutti i clienti: con la versione 24.6 (13 giugno 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Condividi moduli personalizzati e campi personalizzati nella finestra di progettazione moduli personalizzati</a></p>
                        [!BADGE In produzione &#x200B;]{type=Informative}
                        <p>È ora possibile condividere sia i moduli personalizzati che i campi personalizzati all’interno del nuovo progettista di moduli. Ciò consente una maggiore collaborazione tra gli utenti sui moduli personalizzati.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 6 giugno 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione per tutti i clienti: 13 giugno</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Aggiungere un nuovo campo personalizzato dall'area Campi</a></p>
                        [!BADGE In produzione &#x200B;]{type=Informative}
                        <p>È ora possibile aggiungere un nuovo campo personalizzato o widget direttamente dall’area Campi di Workfront, senza aprire un modulo personalizzato per la creazione del campo. Questo consente di creare rapidamente campi personalizzati riutilizzabili.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 6 giugno 2024</p>
                            </li>
                            <li>
                                <p>Versione di produzione per tutti i clienti: con la versione 24.7 (18 luglio 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Tipo di campo a discesa a selezione multipla disponibile nella finestra di progettazione del modulo</a></p>
                        [!BADGE In produzione &#x200B;]{type=Informative}
                        <p>Per semplificare la definizione dei campi a discesa, è stato aggiunto il campo a discesa Selezione multipla al designer del modulo personalizzato. Questo tipo di campo consente agli utenti di scegliere più opzioni da un elenco a discesa.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 4 giugno 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produzione per tutti i clienti: 4 giugno 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Miglioramenti alla gestione finanziaria

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Funzionalità</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Date di rilascio</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Campi delle spese fatturabili e non fatturabili disponibili per progetti e attività</a></p>
                        [!BADGE In produzione &#x200B;]{type=Informative}
                        <p>Per semplificare la visualizzazione dei tipi di spesa, le spese sono state suddivise in spese fatturabili e non fatturabili per progetti e attività. Sono disponibili i seguenti campi da aggiungere alle viste e ai rapporti:</p>
                        <ul>
                            <li><p>Costo spese fatturabile pianificabile</p></li>
                            <li><p>Costo spese pianificato non fatturabile</p></li>
                            <li><p>Costo spese non fatturabile effettivo</p></li>
                            <li><p>Costo spese non fatturabile effettivo</p></li>
                        </ul>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 10 maggio 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produzione per tutti i clienti: 10 maggio 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### Miglioramenti dell’integrazione

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Funzionalità</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Date di rilascio</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Miglioramenti di Workfront per Experience Manager Assets e Assets Essentials</a></p>
                        [!BADGE In produzione &#x200B;]{type=Informative}
                        <p>Sono stati apportati i seguenti miglioramenti alle integrazioni Workfront per Experience Manager Assets e Assets Essentials:</p>
                        <ul>
                            <li><p>L’integrazione ora supporta GCP come provider di servizi cloud. In precedenza, AWS e Azure erano supportati.</p></li>
                            <li><p>Il limite di dimensione per i file inviati ad Experience Manager tramite l’integrazione è aumentato a 30 GB. In precedenza, il limite era di 5 GB.</p></li>
                        </ul>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 27 giugno 2024</p>
                            </li>
                            <li>
                                <p>Produzione per tutti i clienti: con la versione 24.7 (18 luglio 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### Miglioramenti al progetto

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Funzionalità</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Date di rilascio</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Modifica l'attività e il problema Conferma data e condizione dall'intestazione o dalla sezione Dettagli</a></p>
                        [!BADGE In produzione &#x200B;]{type=Informative}
                        <p>Per semplificare l’aggiornamento di attività e problemi, ora sono stati aggiunti i campi Conferma data e Condizione come opzioni da aggiungere alle intestazioni delle attività e dei problemi e alla sezione Dettagli in un modello di layout. Gli utenti possono ora aggiornare questi campi dall’intestazione o dalla sezione Details (Dettagli) di una pagina, quando sono assegnati al modello di layout modificato.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 30 maggio 2024</p>
                            </li>
                            <li>
                                <p>Produzione per rilascio rapido: con la versione 24.6 (13 giugno 2024)</p>
                            </li>
                            <li>
                                <p>Versione di produzione per tutti i clienti: con la versione 24.7 (18 luglio 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Altre assegnazioni rilevanti aggiunte al flusso di lavoro Nuova attività</a></p>
                        [!BADGE In produzione per rilascio rapido &#x200B;]{type=Positive}
                        <p>È stata aggiunta la stessa funzionalità per assegnazioni intelligenti più rilevanti al campo Assegnazioni della casella Nuova attività quando si aggiunge un'attività a un progetto e in un elenco di attività di progetto.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 13 febbraio 2024</p>
                            </li>
                            <li>
                                <p>Produzione per rilascio rapido: con la versione 24.5 (16 maggio 2024)</p>
                            </li>
                        </ul>
                    <p><i>Questa funzione è stata rimossa dall’anteprima e dalla produzione con rilascio rapido.</i></p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Altre assegnazioni avanzate rilevanti</a></p>
                        [!BADGE In produzione per rilascio rapido &#x200B;]{type=Positive}
                        <p>È stato modificato l’algoritmo utilizzato da Workfront per calcolare e suggerire assegnazioni intelligenti per le attività. Il nuovo algoritmo si applica nelle seguenti aree di Workfront in cui si assegna un’attività: elenchi di attività, area Assegnazioni nell’intestazione dell’attività, Home e il pannello Riepilogo.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 21 dicembre 2023</p>
                            </li>
                            <li>
                                <p>Produzione per rilascio rapido: con la versione 24.5 (16 maggio 2024)</p>
                            </li>
                        </ul>
                    <p><i>Questa funzione è stata rimossa dall’anteprima e dalla produzione con rilascio rapido.</i></p>
                    </td>
                 </tr>
           </tbody>
        </table>

### Miglioramenti delle bozze

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Funzionalità</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Date di rilascio</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti di sicurezza per il visualizzatore di bozze per il desktop</a></p>
                        [!BADGE In produzione &#x200B;]{type=Informative}
                        <p>L’aggiornamento di sicurezza 2.1.35 di Workfront Proof Desktop Proofing Viewer fornisce correzioni di bug di sicurezza per le vulnerabilità identificate nelle versioni precedenti.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 4 luglio 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produzione per tutti i clienti: 4 luglio 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### Miglioramenti alla gestione delle risorse

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Funzionalità</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Date di rilascio</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md">Indisponibilità ora riportata nel Bilanciatore dei carichi di lavoro</a></p>
                        [!BADGE In produzione &#x200B;]{type=Informative}
                        <p>Per regolare facilmente il lavoro quando l’assegnatario principale di un’attività ha programmato un’indisponibilità, il Bilanciatore dei carichi di lavoro ora riassegna le ore sia agli utenti principali che a quelli secondari quando la sequenza temporale del progetto viene ricalcolata.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 6 giugno 2024</p>
                            </li>
                            <li>
                                <p>Versione di produzione per tutti i clienti: con la versione 24.7 (18 luglio 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Altri miglioramenti

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Funzionalità</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Date di rilascio</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Modifica back-end alle guide interne al prodotto</a></p>
                        <p>Stiamo implementando un cambiamento tecnologico per le nostre guide interne al prodotto nelle prossime settimane. Anche se abbiamo cercato di ridurre al minimo l’impatto di questa transizione, alcuni utenti potrebbero trovare guide che hanno già visto.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Produzione per tutti i clienti: incrementale fino a metà agosto 2024</p>
                            </li>
                         </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Esperienza unificata Adobe ora disponibile per altre organizzazioni Workfront</a></p>
                        [!BADGE In produzione &#x200B;]{type=Informative}
                        <p>Per consentire alle organizzazioni di accedere ai vantaggi dell’esperienza unificata di Adobe, abbiamo iniziato a renderla disponibile ai clienti Workfront esistenti. </p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 20 giugno 2024</p>
                            </li>
                            <li>
                                <p>Produzione per clienti specifici: con la versione 24.7 (18 luglio 2024)</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;">Adobe Unified Shell è stato reso disponibile in un rollout graduale. Con le versioni 24.10 e 25.1, in Adobe Unified Shell verranno integrate ulteriori organizzazioni. </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Pulsante? rimosso dalla barra di navigazione principale</a></p>
                        [!BADGE In produzione &#x200B;]{type=Informative}
                        <p>Per unificare l’esperienza per gli utenti non su Unified Shell, è stato rimosso il pulsante Aiuto sulla barra di navigazione principale. Questo pulsante, non disponibile per gli utenti di Unified Shell, era collegato alla documentazione di Workfront ed era ridondante con un pulsante Aiuto simile disponibile per tutti gli utenti nel menu principale.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 6 giugno 2024</p>
                            </li>
                            <li>
                                <p>Versione di produzione per tutti i clienti: con la versione 24.7 (18 luglio 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Esperienza interfaccia utente migliorata per gli utenti con accesso limitato agli oggetti</a></p>
                        [!BADGE In produzione &#x200B;]{type=Informative}
                        <p>Quando un utente non ha accesso a un oggetto, visualizzerà "Nessun accesso" in qualsiasi punto del nome dell’oggetto in Workfront. Questa esperienza migliorata si applica anche all’API Workfront.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 27 marzo 2024</p>
                            </li>
                            <li>
                                <p>Produzione per rilascio rapido: con la versione 24.5 (16 maggio 2024)</p>
                            </li>
                            <li>
                                <p>Produzione per rilascio trimestrale: con il rilascio 24.7 (18 luglio 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti look-and-feel durante l’intervallo di tempo del terzo trimestre 2024</a></p>
                        <p>Aggiornamenti minori al look and feel di varie aree dell’applicazione Adobe Workfront vengono effettuati entro l’arco temporale del terzo trimestre 2024. Consulta le singole note sulla versione per specifiche date di rilascio.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: nell’arco temporale della versione del terzo trimestre 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: consulta le note sulla versione per date specifiche</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>

## Notifiche

### Miglioramenti apportati a Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili in produzione a una cadenza che esula dalla pianificazione del rilascio del terzo trimestre 2024. Per ulteriori informazioni sulle funzionalità più recenti, vedere [Attività di Adobe Workfront Fusion release](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Miglioramenti di Workfront Scenario Planner

A questo punto della versione, non sono presenti aggiornamenti di Scenario Planner. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### Miglioramenti di Workfront Proof

A questo punto della versione, non ci sono aggiornamenti per Workfront Proof. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### Miglioramenti agli obiettivi di Workfront

A questo punto della versione, non ci sono aggiornamenti per gli Obiettivi di Workfront. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### API versione 18

Per API versione 18, abbiamo modificato alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

Per informazioni sulle novità e sugli aggiornamenti, vedere [Novità della versione API 18](/help/quicksilver/wf-api/api/new-api-version-18.md).

Per informazioni sulle versioni API, vedere [Controllo delle versioni e pianificazione del supporto API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Aggiornamenti di manutenzione per Workfront

Per informazioni sugli aggiornamenti di manutenzione effettuati durante la versione del terzo trimestre 2024, vedi [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/it/docs/workfront-known-issues/releases/current-updates).

### Aggiornamenti dei corsi di formazione

Scopri gli ultimi aggiornamenti apportati a programmi di apprendimento, percorsi di apprendimento, video e guide per ogni versione di Adobe Workfront. Per ulteriori informazioni, vedere la sezione &quot;Novità&quot; della [pagina delle esercitazioni di Workfront](https://experienceleague.adobe.com/it/docs/workfront-learn/tutorials-workfront/home).
