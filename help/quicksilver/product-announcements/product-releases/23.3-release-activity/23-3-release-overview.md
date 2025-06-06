---
title: Panoramica sulla versione 23.3
description: Panoramica sulla versione 23.3
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 441d84d6-6c40-4a03-967e-836cf78c8fc1
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '2799'
ht-degree: 0%

---

# Panoramica sulla versione 23.3

Questa pagina fornisce informazioni sulle funzionalità incluse nella versione 23.3 di. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione con la versione 23.3 del 20 e 21 luglio 2023.

Il webinar sulla versione 23.3 di è stato pubblicato il 29 giugno 2023. Puoi [registrarti al webinar per visualizzare una registrazione on-demand qui](https://webinars.on24.com/adobe_workfront/whatsnewin233?partnerref=exlreleaseoverview).

<span class="preview">Le funzioni off-cycle (quelle rilasciate in produzione prima della data di rilascio della versione 23.3) sono evidenziate in giallo.</span>

>[!IMPORTANT]
>
>La versione 23.3 include l’opzione per spostare l’organizzazione alle versioni mensili. Pertanto, Workfront sta modificando lo schema di numerazione delle versioni in modo da tenere conto delle versioni mensili e trimestrali.
>
>* Se sei sulla traccia **versione rapida (mensile)**, la versione dopo la versione 23.3 sarà **23.8**, il 31 agosto 2023.
>* Se sei sulla traccia della versione **trimestrale**, la versione dopo la versione 23.3 sarà **23.10**, nella settimana del 26 ottobre 2023.
> 
> I rilasci trimestrali includeranno funzionalità da tre rilasci mensili. Ad esempio, la versione trimestrale 23.10 includerà le funzionalità rilasciate nelle versioni mensili 23.8, 23.9 e 23.10.
>
>I rilasci mensili e trimestrali dovrebbero essere disponibili l&#39;ultimo giovedì del mese.
>
>| Versione mensile | Versione trimestrale |
>|----|----|
>| <ul><li>23.8 (31 agosto 2023)</li><li>23.9 (28 settembre 2023)</li><li>23.10 (26 ottobre 2023)</li></ul> | <ul><li>23.10 (Settimana del 26 ottobre 2023)</li></ul> |
>| <ul><li>Nessuna versione (novembre 2023)</li><li>Nessuna versione (dicembre 2023)</li><li>24.1 (gennaio 2024)</li></ul> | <ul><li>24.1 (gennaio 2024)</li></ul> |
>
>Per ulteriori informazioni sul processo di rilascio rapido, vedere [Attivare o disattivare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Miglioramenti di Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Miglioramenti Agile](#agile-enhancements)
* [Miglioramenti di Financial Management](#financial-management-enhancements)
* [Miglioramenti dell’integrazione](#integration-enhancements)
* [Miglioramenti al progetto](#project-enhancements)
* [Miglioramenti per dispositivi mobili](#mobile-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Cicli di rilascio più rapidi per Workfront</a></p>
                        <p>Per consentirti di ricevere più rapidamente nuovi aggiornamenti e funzioni dei prodotti Workfront, abbiamo aggiunto la possibilità di abilitare cicli di rilascio più rapidi. Ora puoi scegliere di far sì che la tua organizzazione riceva le versioni di Workfront con una frequenza maggiore di una volta a trimestre. Il ciclo di rilascio trimestrale sarà ancora disponibile per le organizzazioni che preferiscono versioni meno frequenti.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 22 giugno 2023</p>
                            </li>
                            <li>
                                <p>Versione di produzione: con la versione 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Controllo a livello di gruppo disponibile per la preferenza relativa alle ore e alla scheda orario "Dove gli utenti possono registrare l'ora"</a></p>
                        <p>L’amministratore di sistema ora può bloccare e sbloccare la scheda orario e la preferenza orario "Dove gli utenti possono registrare l’ora". Quando questa preferenza viene sbloccata, gli amministratori di gruppi possono configurare le impostazioni "Where users can log time" (Dove gli utenti possono registrare il tempo) separatamente per ciascun gruppo.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 4 maggio 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: 18 maggio 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Visualizza gli indicatori logici e ignora gli indicatori logici e le regole visualizzati nella versione beta di Progettazione moduli</a></p>
                        <p>La versione beta pubblica del designer del modulo è stata riabilitata in Anteprima e produzione il 21 luglio 2023. Inoltre, è ora possibile visualizzare le regole logiche esistenti create nei moduli personalizzati precedenti all’interno del progettista del modulo.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 21 luglio 2023</p>
                            </li>
                            <li>
                                <p>Versione di produzione: 21 luglio 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Miglioramenti Agile

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">La visualizzazione Agile di un progetto mostra una bacheca kanban</a></p>
                        <p>La visualizzazione Agile di un progetto ora include funzionalità aggiuntive per filtrare, raggruppare e ordinare il lavoro in una bacheca kanban. Il nuovo design flessibile della vista include una solida funzione di ricerca e la possibilità di aggiungere nuove attività al progetto direttamente dalla bacheca.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 29 giugno 2023</p>
                            </li>
                            <li>
                                <p>Versione di produzione per tutti i clienti: con la versione 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Ordina per colonne della bacheca</a></p>
                        <p>È stata aggiunta la possibilità di ordinare le schede nelle colonne di una bacheca. Quando si seleziona un'opzione in base alla quale eseguire l'ordinamento, vengono ordinate tutte le colonne. Non è possibile ordinare una singola colonna e la colonna backlog o acquisizione non è ordinata.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 22 giugno 2023</p>
                            </li>
                            <li>
                                <p>Versione di produzione per tutti i clienti: con la versione 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>                             
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Modalità scura ora disponibile sulle schede madri Adobe Workfront</a></p>
                        <p>Ora è possibile visualizzare tutte le schede madri e i flussi di lavoro in modalità scura. La nuova impostazione è disponibile tramite le preferenze nel dashboard Bacheche.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 22 giugno 2023<span style="color: #ff0000;"> Questa funzione è stata rimossa dall'anteprima e non verrà rilasciata con 23.3.</span></p>
                            </li>
                            <li>
                                <p>Versione di produzione per tutti i clienti: N/D</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Obiettivi disponibili per le iterazioni del flusso di lavoro nelle schede madri Adobe Workfront</a></p>
                        <p>È stata aggiunta la possibilità di aggiungere obiettivi a un’iterazione, senza dover elencare gli obiettivi su una scheda. Gli obiettivi vengono aggiunti in un formato elenco di controllo e possono essere contrassegnati come completati. L’area delle metriche in alto a destra dell’iterazione mostra quanti obiettivi esistono e quanti sono stati completati.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 22 giugno 2023<span style="color: #ff0000;"> Questa funzione è stata rimossa dall'anteprima e non verrà rilasciata con 23.3.</span></p>
                            </li>
                            <li>
                                <p>Versione di produzione per tutti i clienti: N/D</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Aggiungi commenti alle schede nelle bacheche</a></p>
                        <p>È ora possibile aggiungere commenti alle schede ad hoc e alle schede collegate sulle bacheche e assegnare tag ad altri utenti sui commenti. I commenti sono disponibili nei dettagli della scheda. La funzione di commento per le bacheche utilizza la nuova esperienza di commento di Adobe Workfront.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 15 giugno 2023</p>
                            </li>
                            <li>
                                 <p>Versione di produzione per consenso anticipato: 22 giugno 2023 <span style="color: #ff0000;"> Questa funzione è disponibile in produzione in questa data solo tramite consenso anticipato per le schede madri Workfront.</span></p>
                                <p>Versione di produzione per tutti i clienti: con la versione 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Miglioramenti al gestore di tag delle bacheche</a></p>
                        <p>È stata migliorata l’interfaccia di Gestione tag, che consente di creare rapidamente nuovi tag e applicarli alle schede. Puoi anche creare tag per i flussi di lavoro.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 19 maggio 2023</p>
                            </li>
                            <li>
                                 <p><span class="preview">Versione di produzione: 19 maggio 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Filtri semplici disponibili nelle colonne di acquisizione della scheda</a></p>
                        <p>Sono stati aggiunti filtri semplificati all’impostazione della colonna Acquisizione per consentirti di definire più rapidamente la colonna Acquisizione. I filtri disponibili sono progetti Workfront e assegnazioni per team o utente. Se lo desideri, puoi passare ai filtri avanzati.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 10 maggio 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versione di produzione per il consenso anticipato: 10 maggio 2023 <span style="color: #ff0000;"> Questa funzione è disponibile in produzione in questa data solo tramite il consenso anticipato per le schede madri Workfront.</span></p>
                                <p>Versione di produzione per tutti i clienti: con la versione 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Filtri semplici aggiunti al modello di bacheca dinamica</a></p>
                        <p>I filtri nel modello della bacheca dinamica sono stati semplificati per consentire di creare una bacheca più rapidamente.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 27 aprile 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versione di produzione per il consenso anticipato: 28 aprile 2023 <span style="color: #ff0000;"> Questa funzione è disponibile in produzione in questa data solo tramite il consenso anticipato per le schede madri Workfront.</span></p>
                                <p>Versione di produzione per tutti i clienti: con la versione 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Modello per bacheca dinamica</a></p>
                        <p>Per le bacheche autonome è ora disponibile un nuovo modello, la bacheca dinamica. Questo modello non è disponibile per le bacheche all’interno di un flusso di lavoro.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 20 aprile 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versione di produzione per il consenso anticipato: 28 aprile 2023 <span style="color: #ff0000;"> Questa funzione è disponibile in produzione in questa data solo tramite il consenso anticipato per le schede madri Workfront.</span></p>
                                <p>Versione di produzione per tutti i clienti: con la versione 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Migrazione delle schede Kanban del team agile alle bacheche</a></p>
                        <p>Un nuovo pulsante <b>Aggiungi alle bacheche</b> su bacheche Kanban del team agile consente di aggiungere tutte le schede dalla bacheca Kanban a una bacheca Workfront. Puoi scegliere di creare una nuova bacheca Workfront o aggiungere le schede a una bacheca esistente.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 20 aprile 2023<br /></p>
                            </li>
                            <li>
                                 <s><p>Versione di produzione per il consenso anticipato: 28 aprile 2023 <span style="color: #ff0000;"> Questa funzione è disponibile in produzione in questa data solo tramite il consenso anticipato per le schede madri Workfront.</span></p></s>
                                 </li>
                                 <li>
                                <p><span class="preview">Versione di produzione per tutti i clienti: 18 maggio 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Navigazione a sinistra aggiunta ai dettagli delle schede in Bacheche</a></p>
                        <p>Man mano che più opzioni di campo vengono aggiunte alle schede sulle Schede Workfront, i dettagli della scheda si sono allungati. Un nuovo pannello di navigazione a sinistra dei dettagli della scheda ti consente di selezionare una sezione e di passare automaticamente a quel gruppo di campi.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 20 aprile 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione per tutti i clienti: 27 aprile 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Notifiche e preferenze e-mail per le bacheche</a></p>
                        <p>Le notifiche e-mail sono ora disponibili per le bacheche di Adobe Workfront. Le notifiche sono attivate per impostazione predefinita e puoi selezionare nelle preferenze quali e-mail desideri ricevere. Riceverai un’e-mail quando verrai aggiunto a una bacheca e quando ti verrà assegnata una scheda.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 13 aprile 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versione di produzione per il consenso anticipato: 13 aprile 2023 <span style="color: #ff0000;"> Questa funzione è disponibile in produzione in questa data solo tramite il consenso anticipato per le schede madri Workfront.</p>
                                <p>Versione di produzione per tutti i clienti: con la versione 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Miglioramenti di Financial Management

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-finance-enhancements.md" class="MCXref xref" xrefformat="{para}">Tariffe di fatturazione e costi effettivi per data</a></p>
                        <p>Le tariffe di costo e fatturazione effettive per data sono ora disponibili per gli oggetti società, utente e mansione in Workfront. Quando a un progetto vengono applicati i tassi di validità della data e le ore vengono registrate nelle attività del progetto, i costi e i ricavi vengono calcolati utilizzando i tassi specificati per ogni periodo di tempo.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 29 giugno 2023</p>
                            </li>
                            <li>
                                <p>Versione di produzione per i clienti della versione Fast: da annunciare, dopo la versione di produzione 23.3</p>
                                <p>Versione di produzione per tutti i clienti: da annunciare<br>
                                La funzione di sostituzione della percentuale di assegnazione è stata temporaneamente disabilitata in Anteprima dal 30 giugno al 13 luglio 2023.</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">È ora disponibile la nuova integrazione di Google Workspace</a></p> 
                        <p>Una nuova integrazione di Google Workspace è ora disponibile nel marketplace Google. La nuova integrazione esegue l’autenticazione utilizzando OAuth2 e sostituisce l’integrazione precedente.</p><p>La precedente integrazione di Google Workspace è ora obsoleta e verrà disinstallata automaticamente.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Anteprima versione: N/D</p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: 27 giugno 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Le integrazioni Adobe Creative Cloud ora supportano più utenti assegnati</a></p> 
                        <p>L'integrazione di Adobe Creative Cloud ora supporta la possibilità di scegliere tra "Fine con la parte" e "Completo" (o "Risolto") quando a un'attività o a un problema sono assegnati più utenti.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Anteprima versione: N/D</p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: 22 giugno 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Visualizza e gestisci le notifiche Workfront dai plug-in di Workfront for Creative Cloud</a></p> 
                        <p>Per semplificare la ricezione delle notifiche necessarie, è possibile visualizzare e gestire le notifiche di Workfront senza uscire da Adobe Creative Cloud. Ora puoi visualizzare le notifiche, nonché accedere agli elementi di lavoro e ai commenti relativi a tali notifiche direttamente dalla finestra del plug-in Workfront all’interno dell’applicazione Creative Cloud.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Anteprima versione: N/D</p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: 22 giugno 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
 <!--               <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Improved experience when moving a document to a linked folder with drag and drop</a></p> 
                        <p>We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder. </p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: June 7, 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: June 15, 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>-->
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Creazione automatica di cartelle collegate in Adobe Experience Manager Assets durante la creazione di un progetto</a></p>
                        <p>Con il nuovo flusso di lavoro Crea cartella collegata per l’integrazione Adobe Experience Manager, puoi configurare l’integrazione con un percorso a una cartella Adobe Experience Manager Assets. Quando l’integrazione viene aggiunta a un modello di progetto, tutti i progetti creati dal modello creano automaticamente una sottocartella collegata in Experience Manager Assets nella cartella specificata. </p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 11 maggio 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: 24 maggio 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Mappa i valori dei campi di Workfront ai tag in Experience Manager Assets</a></p>
                        <p>Ora è possibile categorizzare e trovare rapidamente le risorse in base ai dati provenienti da Workfront. Puoi mappare questi dati come parte della configurazione dei metadati nell’integrazione di Workfront for Experience Manager Assets.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 10 maggio 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: 10 maggio 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Mappatura dei campi di Workfront con campi di metadati Experience Manager Assets personalizzati</a></p>
                        <p>Con l’integrazione nativa, ora è possibile mappare i campi Workfront nativi e incorporati ai campi dello schema di metadati personalizzati in Experience Manager Assets as a Cloud Service.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 10 maggio 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: 10 maggio 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Regola le impostazioni del modello di flusso di lavoro per bozza automatizzata con Adobe Workfront per Creative Cloud</a></p>
                        <p>È ora possibile modificare le impostazioni del modello di flusso di lavoro automatico esistente direttamente in Creative Cloud.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 27 aprile 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: 27 aprile 2023</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Approvazioni nuovi documenti</a> </p>
                        <p>Le approvazioni dei documenti vengono riprogettate in un rollout graduale che verrà reso disponibile a più utenti con ogni versione.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 31 maggio 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: 14 giugno 2023</span></p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">Questa funzione fa parte di un rilascio graduale ed è attualmente disponibile solo per clienti specifici.</span></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Pulsante Nuova condivisione</a> </p>
                        <p>L’opzione Condividi è stata rimossa dal menu Altro per consentire la condivisione di progetti, attività e problemi in modo più intuitivo.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 22 giugno 2023<br /></p>
                            </li>
                            <li>
                                <p>Versione di produzione: con la versione 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Miglioramenti per dispositivi mobili

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}">Nuova funzionalità di bozza nell'app mobile Workfront</a> </p>
                        <p>Con la rimozione dell’app Workfront Proof autonoma nella versione 23.10 (ottobre 2023), l’app mobile primaria di Workfront ha avuto funzioni di verifica aggiunte per consentire il proseguimento delle verifiche su dispositivi mobili.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Anteprima versione: N/D</p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: disponibile in Apple App Store e Google Play Store il 21 giugno 2023</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nuova esperienza Home</a></p>
                        <p>Per consentire agli utenti di tutti i tipi di utilizzare al meglio Workfront per le loro esigenze specifiche, Home ha ricevuto un aggiornamento importante! La nuova esperienza Home offre la personalizzazione visiva e dei contenuti per la home page, offrendo la flessibilità di visualizzare solo le informazioni più rilevanti per il tuo lavoro.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 23 giugno 2023</p>
                            </li>
                            <li>
                                <p>Versione di produzione: con la versione 23.3</p>
                            </li>
                        </ul>
                    </td>
                 </tr>                                 
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nuova esperienza di aggiunta di commenti per altri oggetti</a> </p>
                        <p>La nuova esperienza di aggiunta di commenti sarà disponibile per i seguenti oggetti, poco dopo la versione 23.3 di in Produzione: attività modello, modelli, schede orario, team, utenti, programmi, portfolio.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: da annunciare, dopo il rilascio della versione 23.3 Production</p>
                            </li>
                            <li>
                                <p>Versione di produzione per i clienti della versione Fast: da annunciare, dopo la versione di produzione 23.3 </p>
                                <p>Versione di produzione per tutti i clienti: con la versione 23.10 (ottobre 2023)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>                
            <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nuova esperienza Beta con commenti per progetti, attività e documenti</a> </p>
                        <p>La nuova esperienza Beta per la creazione di commenti è ora disponibile per progetti, attività e documenti. Prima di questo aggiornamento, l’esperienza con Beta per la creazione di commenti era disponibile solo per problemi e obiettivi.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 1 giugno 2023<br /></p>
                            </li>
                            <li>
                                <p>Versione di produzione: con la versione 23.3</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">I profili senza avatar ora visualizzano le iniziali utente</a></p>
                        <p>Per facilitare la ricerca di utenti specifici all’interno di elenchi di grandi dimensioni, i profili senza avatar personalizzati ora visualizzano le iniziali dell’utente su uno sfondo colorato in elenchi e rapporti legacy. Si tratta di una modifica cosmetica minore e non si applica se è già in uso una foto avatar o se l’utente è disattivato.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 20 aprile 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: 4 maggio 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md" class="MCXref xref" xrefformat="{para}">Nuovi miglioramenti dell'esperienza beta per il commento</a></p>
                        <p>I miglioramenti alla sezione Aggiornamenti sono stati resi disponibili entro l’arco temporale della versione 23.3 per la nuova esperienza beta di creazione di commenti. Salvo diversa indicazione, questi miglioramenti saranno resi disponibili nell’ambiente di produzione con la versione 23.3.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: nell’arco temporale della versione 23.3<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: con la versione 23.3 (se non diversamente specificato)</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md" class="MCXref xref" xrefformat="{para}">Nuovi miglioramenti all'esperienza del dashboard Canvas</a></p>
                        <p>I miglioramenti al dashboard di Canvas saranno disponibili entro l’intervallo di tempo della versione 23.3. Salvo diversa indicazione, questi miglioramenti saranno resi disponibili nell’ambiente di produzione con la versione 23.3. 
 </p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 5 giugno 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: 5 giugno 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti look-and-feel durante l'intervallo di tempo della versione 23.3</a></p>
                        <p>Aggiornamenti minori al look and feel di varie aree dell’applicazione Adobe Workfront vengono effettuati entro l’arco temporale della versione 23.3. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione almeno 2 settimane dopo il rilascio in anteprima.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: nell’arco temporale della versione 23.3</p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: almeno 2 settimane dopo il rilascio in anteprima (se non diversamente specificato)</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>   
           </tbody>
        </table>

## Notifiche

### Miglioramenti apportati a Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili in produzione a una cadenza al di fuori della pianificazione della versione 23.3. Per ulteriori informazioni sulle funzionalità più recenti, vedere [Attività di Adobe Workfront Fusion release](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Miglioramenti di Workfront Scenario Planner

A questo punto della versione, non sono presenti aggiornamenti di Scenario Planner. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### Miglioramenti di Workfront Proof

Nuove funzioni in arrivo in Workfront Proof rilasciate entro l’arco temporale della versione 23.3. Per informazioni su queste nuove funzioni ora disponibili in Anteprima, consulta [Adobe Workfront Proof con versione 23.3](/help/quicksilver/product-announcements/product-releases/workfront-proof-release-activity/proof-23-3-release/proof-23-3-overview.md).

### Miglioramenti agli obiettivi di Workfront

Nuove funzioni in arrivo per il rilascio di Workfront Goals entro l’arco temporale di rilascio 23.3. Per informazioni su queste nuove funzioni ora disponibili in Anteprima, vedi [Obiettivi di Adobe Workfront con la versione 23.3](/help/quicksilver/product-announcements/product-releases/goals-release-activity/goals-23-3-release/goals-23-3-release.md).

### API versione 16

Per API versione 16, abbiamo modificato alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

Per informazioni sulle novità e sugli aggiornamenti, vedere [Novità della versione API 16](/help/quicksilver/wf-api/api/new-api-version-16.md).

Per informazioni sulle versioni API, vedere [Controllo delle versioni e pianificazione del supporto API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Aggiornamenti di manutenzione per Workfront

Per informazioni sugli aggiornamenti di manutenzione apportati durante la versione 22.3, vedere [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/it/docs/workfront-known-issues/releases/current-updates).

### Aggiornamenti dei corsi di formazione

Scopri gli ultimi aggiornamenti apportati a programmi di apprendimento, percorsi di apprendimento, video e guide per ogni versione di Adobe Workfront. Per ulteriori informazioni, vedere la sezione &quot;Novità&quot; della [pagina delle esercitazioni di Workfront](https://experienceleague.adobe.com/it/docs/workfront-learn/tutorials-workfront/home).

### Funzionalità presto rimossa da Workfront

Le seguenti funzionalità verranno presto rimosse da Workfront:

#### L’app mobile Proof è diventata obsoleta con la versione 23.10 (ottobre 2023)

Con la versione 23.10 (ottobre 2023), l’app mobile Proof diventerà ufficialmente obsoleta. L’app mobile generale di Workfront è stata migliorata con nuove funzionalità di verifica (per ulteriori informazioni, consulta la nota sulla versione in Miglioramenti di Workfront Mobile) e si consiglia agli utenti di iniziare a utilizzarla per il lavoro di verifica il prima possibile.

L’app mobile Workfront richiede un accesso a Workfront. Gli utenti esterni e gli ospiti possono continuare a utilizzare l’app Bozza per il lavoro di verifica; tuttavia, non è più supportata e non sarà più disponibile con la versione 23.10 (ottobre 2023).


<!-- HTML you might need

New table

### add product area name

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="ADD LINK" class="MCXref xref" xrefformat="{para}">Title</a><span style="color: #ff0000;"> New in Preview!</span></p>
                        <p>Body</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release:<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

New row for table 

<tr>
  <td>
    <a href="ADD%20LINK">Title</a> New in Preview!
    <p>Body</p>
  </td>
  <td>
    <p><strong>Available on these dates:</strong></p>
    <ul>
      <li>
        <p>Preview release:</p>
      </li>
      <li>
        <p>Production release:</p>
      </li>
    </ul>
  </td>
</tr>


New in preview, prod, and coming soon text

<span style="color: #ff0000;"> New in Preview!</span>
<span style="color: #ff0000;"> New in Production!</span>
<span style="color: #ff0000;"> Coming soon!</span>


Test for boards early access stuff

Production release for early opt-in: March 2, 2023 This feature is available in Production only through the early feature opt-in for Workfront Boards.

Production release for all customers: With the 23.2 release

-->
