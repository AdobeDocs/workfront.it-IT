---
title: Panoramica sulla versione 23.2
description: Panoramica sulla versione 23.2
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b0e2ce08-d9f7-4fb5-b35c-ba979ab9d03e
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '2769'
ht-degree: 0%

---

# Panoramica sulla versione 23.2

Questa pagina fornisce informazioni sulle funzionalità incluse nella versione 23.1 di. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione con la versione 23.2 del 6 e 7 aprile 2023.

Per suggerimenti sulla preparazione della prossima versione, consulta [Prepararsi per una versione trimestrale di Adobe Workfront](/help/quicksilver/product-announcements/product-releases/release-readiness.md).

## Webinar sulla versione

Al posto del webinar sulla versione, ti invitiamo a registrarti, ad Adobe Summit, per guardare le seguenti sessioni su Workfront:

[Esperienze di impatto: dalla creazione di contenuti alla personalizzazione](https://reg.adobe.com/flow/adobe/as23/sessions/page/catalog/session/1661982243928001D5Z9) il 21 marzo 2023, per scoprire nuovi modi di creare, gestire e personalizzare i contenuti e fornire esperienze di impatto con una maggiore efficienza. Questa sessione verrà trasmessa in streaming live per i tipi di pubblico virtuali.

[Il futuro di Adobe Workfront](https://reg.adobe.com/flow/adobe/as23/sessions/page/catalog/session/1661982239896001DoHU) il 23 marzo 2023, per scoprire la visione di Workfront e del suo ruolo all’interno dell’ecosistema Adobe e dare un’occhiata alla roadmap futura. Questa sessione verrà registrata e sarà disponibile in seguito come contenuto on-demand.

<span class="preview">Le funzioni off-cycle (quelle rilasciate in produzione prima della data di rilascio della versione 23.2) sono evidenziate in giallo.</span>

## Miglioramenti di Adobe Workfront

* [Miglioramenti per gli amministratori](#administrator-enhancements)
* [Miglioramenti Agile](#agile-enhancements)
* [Miglioramenti alla gestione dei progetti](#project-management-enhancements)
* [Miglioramenti alla gestione delle risorse](#resource-management-enhancements)
* [Miglioramenti ai report e alle dashboard](#reports-and-dashboards-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Mappare i valori dei campi di Workfront ai tag in Experience Manager Assets</a>
                        <p>Ora è possibile categorizzare e trovare rapidamente le risorse in base ai dati provenienti da Workfront.  Puoi mappare questi dati come parte della configurazione dei metadati nell’integrazione di Workfront for Experience Manager Assets.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Anteprima versione: N/D<br /></p>
                            </li>
                            <li>
                                 <p>Versione di produzione: 30 marzo 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Creare moduli personalizzati con la nuova versione beta di Progettazione moduli</a>
                        <p>Il nuovo progettista di moduli dispone di una nuova area di lavoro in stile area di lavoro che consente di visualizzare contemporaneamente i campi, l'area di lavoro e le impostazioni dei campi.</p>
                        <p>Con il nuovo form designer è stata aggiunta la possibilità di 
                        <ul>
                        <li><strong>Copiare un campo</strong>: ora puoi copiare i campi esistenti facendo clic sull’icona Copia sui campi direttamente dall’area di lavoro.</li>
                        <li><strong>Usa una sezione predefinita</strong>: se il creatore del modulo non ha aggiunto una sezione nella parte superiore del modulo, nell’area di lavoro è ora visibile una sezione predefinita che consente agli utenti di regolare le autorizzazioni per i campi ai quali non è assegnata alcuna sezione personalizzata. </li>
                        <li><strong>Modificare le dimensioni per il testo descrittivo</strong>: ora puoi assegnare dimensioni piccole, medie o grandi ai campi Testo descrittivo. È inoltre possibile utilizzarli nella stessa riga con altri campi. <span style="color: #ff0000;"> La modifica della dimensione del testo descrittivo è stata temporaneamente posticipata ma sarà presto disponibile.</span></li> 
                        </ul>
                        </p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 9 marzo 2023</p>
                            </li>
                            <li>
                                 <p>Versione di produzione: con la versione 23.2<br />
                                 <span style="color: #ff0000;">La versione beta di Forms Designer è stata temporaneamente disabilitata in Anteprima e produzione dal 24 maggio al 21 luglio 2023.</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Rinomina pin nel modello di layout</span></a>
                        <p>È ora possibile rinominare i pin di un modello di layout in modo che siano più significativi per gli utenti, invece di utilizzare il nome predefinito per la pagina bloccata. I pin creati dagli amministratori vengono visualizzati per tutti gli utenti assegnati al modello di layout e gli utenti non possono rinominarli.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 9 febbraio 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versione di produzione: con la versione 23.2</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Aggiungere attività e problemi dai dettagli oggetto a una bacheca Workfront o a un flusso di lavoro</a></p>
                        <p>Ora è possibile aggiungere attività o problemi esistenti a una scheda Workfront o a un elenco di schede del flusso di lavoro direttamente dai dettagli dell’oggetto. Tutti gli elementi aggiunti a una bacheca diventano schede collegate e tutti gli elementi aggiunti a un flusso di lavoro vengono aggiunti all’elenco delle schede come schede non pianificate.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 23 marzo 2023<br /></p>
                            </li>
                            <li>
                                <p>Versione di produzione: con la versione 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr> 
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Funzionalità di iterazione disponibile nelle schede madri Adobe Workfront</a></p>
                        <p>Diverse nuove funzioni disponibili nelle schede madri Workfront consentono di utilizzare la funzionalità Scrum agile. Queste caratteristiche includono:
                        <ul>
                        <li>Flussi di lavoro per il raggruppamento di bacheche relative allo stesso team e per la collaborazione al lavoro</li>
                        <li>Un elenco di schede, o backlog di lavoro, con la possibilità di utilizzare le origini per collegare le schede ad attività e problemi di Workfront</li>
                        <li>Bacheche per la pianificazione delle iterazioni e il processo di iterazione</li>
                        </ul>
                        </p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 17 marzo 2023<br /></p>
                            </li>
                            <li>
                                <p>Versione di produzione: con la versione 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr> 
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Aggiungere attività e problemi da elenchi e report a un elenco di schede del flusso di lavoro</a></p>
                        <p>È ora possibile aggiungere attività o problemi esistenti a un flusso di lavoro in Bacheche Workfront direttamente da una vista elenco o report. Tutti gli elementi aggiunti al flusso di lavoro vengono aggiunti all’elenco delle schede come schede non pianificate.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 17 marzo 2023<br /></p>
                            </li>
                            <li>
                                <p>Versione di produzione: con la versione 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Aggiungere campi personalizzati alle schede di una bacheca</a></p>
                        <p>Ora puoi includere campi personalizzati nelle bacheche Adobe Workfront. Il campo deve essere già stato creato in Workfront. Non puoi progettare e creare nuovi campi personalizzati all’interno di una bacheca.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 17 marzo 2023<br /></p>
                            </li>
                            <li>
                                <p>Versione di produzione: con la versione 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Aggiungere attività e problemi da elenchi e rapporti a una bacheca Workfront</a></p>
                        <p>Ora è possibile aggiungere attività o problemi esistenti a una bacheca Workfront direttamente da una vista a elenco o report. Tutti gli elementi aggiunti alla bacheca diventeranno schede collegate.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 2 marzo 2023<br /></p>
                            </li>
                            <li>
                                <p>Versione di produzione: con la versione 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Registra le ore sulle schede collegate su una bacheca</a></p>
                        <p>Ora è possibile registrare le ore sulle schede collegate, come si farebbe su un'attività o un problema. Per registrare l’ora, è necessario disporre delle autorizzazioni corrette per l’attività o il problema.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 23 febbraio 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versione di produzione per il consenso anticipato: 2 marzo 2023 <span style="color: #ff0000;"> Questa funzione è disponibile in produzione in questa data solo tramite il consenso anticipato per le schede madri Workfront.</span></p>
                                <p>Versione di produzione per tutti i clienti: con la versione 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
              <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Personalizzare la visualizzazione dei campi su una scheda</a></p>
                        <p>È ora disponibile la personalizzazione per configurare quali campi visualizzare su una scheda, sia nella visualizzazione completa quando la scheda è aperta che nella visualizzazione ridotta sulla scheda. Quando si disattiva, un campo non viene visualizzato in nessuna delle due visualizzazioni. È inoltre possibile attivare un campo nella visualizzazione completa e nasconderlo dalla visualizzazione ridotta.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 16 febbraio 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versione di produzione per il consenso anticipato: 23 febbraio 2023 <span style="color: #ff0000;"> Questa funzione è disponibile in produzione in questa data solo tramite il consenso anticipato per le schede madri Workfront.</span></p>
                                <p>Versione di produzione per tutti i clienti: con la versione 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Definisci uno stato predefinito per le schede spostate in una colonna della bacheca</a></p>
                        <p>Ora puoi impostare uno stato predefinito da applicare alle schede spostate in una colonna specifica, selezionando uno stato personalizzato e uno stato di sistema nei criteri delle colonne. Quando sposti una scheda nella colonna, Workfront tenta prima di applicare lo stato personalizzato (ad esempio, In attesa di feedback). Se lo stato personalizzato non è disponibile per tale scheda, Workfront applicherà invece lo stato del sistema (ad esempio, In sospeso). Inoltre, se lo stato dell’attività o del problema connesso viene modificato nello stato personalizzato o di sistema impostato nella policy di colonna, la scheda viene automaticamente spostata nella colonna.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 16 febbraio 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versione di produzione per il consenso anticipato: 23 febbraio 2023 <span style="color: #ff0000;"> Questa funzione è disponibile in produzione in questa data solo tramite il consenso anticipato per le schede madri Workfront.</span></p>
                                <p>Versione di produzione per tutti i clienti: con la versione 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Le raccolte sono ora disponibili nelle bacheche di Adobe Workfront</a></p>
                        <p>Ora puoi creare raccolte nel dashboard delle bacheche. Una raccolta è un gruppo di bacheche per la collaborazione sul lavoro. Dopo aver denominato la raccolta, puoi aggiungere bacheche alla raccolta utilizzando un set di modelli che offrono impostazioni predefinite, ad esempio i nomi delle colonne.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 16 febbraio 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versione di produzione per il consenso anticipato: 23 febbraio 2023 <span style="color: #ff0000;"> Questa funzione è disponibile in produzione in questa data solo tramite il consenso anticipato per le schede madri Workfront.</span></p>
                                <p>Versione di produzione per tutti i clienti: con la versione 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Il campo Stima sulle schede collegate viene mappato sul campo Punti storia sugli oggetti Workfront</a></p>
                        <p>Il campo Stima sulle schede collegate in Bacheche Workfront ora viene mappato sul campo Story Points (Punti storia) per l’oggetto Workfront associato. </p>
                        <p>Il nuovo campo Story Points (Punti storia) è un campo libero modificabile che puoi aggiungere a una visualizzazione in un elenco o in un rapporto per attività o problemi. Non è legato alle ore pianificate o alle assegnazioni del team.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 26 gennaio 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versione di produzione per consenso anticipato: questa funzione è stata posticipata e verrà rilasciata il 9 febbraio. <span style="color: #ff0000;">Questa funzione è disponibile in produzione in questa data solo tramite il consenso anticipato per le schede madri Workfront.</span></p>
                                <p>Versione di produzione per tutti i clienti: con la versione 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Scheda di anteprima nella colonna Acquisizione</a></p>
                        <p>Ora puoi fare clic su una scheda collegata nella colonna Acquisizione per visualizzare una versione di sola visualizzazione del suo contenuto. Non puoi modificare il contenuto della scheda finché questa non viene spostata fuori dalla colonna di acquisizione in un’altra colonna sulla bacheca.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 26 gennaio 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versione di produzione per il consenso anticipato: 2 febbraio 2023 <span style="color: #ff0000;"> Questa funzione è disponibile in produzione in questa data solo tramite il consenso anticipato per le schede madri Workfront.</span></p>
                                <p>Versione di produzione per tutti i clienti: con la versione 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Miglioramenti alla gestione dei progetti

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nuova esperienza durante la modifica in blocco di progetti</a>
                        <p>Per aggiornare l’aspetto dell’esperienza Workfront, è stata riprogettata la casella Modifica progetti, che consente di modificare più progetti contemporaneamente in blocco. Puoi accedere alla nuova casella Modifica progetti quando selezioni più progetti contemporaneamente in un elenco di progetti.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 9 marzo 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Versione di produzione: a partire dal 23 marzo, verrà rilasciata alla produzione in un rollout graduale che verrà completato dopo l’11 maggio 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Esperienza di filtro migliorata generalmente disponibile in Adobe Workfront</a>
                        <p>L’esperienza di filtro migliorata sarà generalmente disponibile e diventerà il generatore di filtri standard in Anteprima il 2 marzo 2023. Anche il rollout graduale in produzione inizierà il 2 marzo, con disponibilità per tutti i clienti nella versione 23.2.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 2 marzo 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Versione di produzione: con la versione 23.2</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Copia ore preventivate durante la copia di un progetto</a>
                        <p>Ora è possibile copiare le ore preventivate nell'area Budget risorse del Business Case o della Programmazione risorse quando si copia un progetto. Prima di questo miglioramento, le ore preventivate per il progetto non venivano trasferite al progetto copiato.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 16 febbraio 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Versione di produzione: 2 marzo 2023 (fuori ciclo)</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-resource-management-enhancements.md" class="MCXref xref" xrefformat="{para}">Introduzione del campo Tempo di lavoro per calcolare con precisione la capacità dell'utente</a>
                        <p>Per consentire ai responsabili delle risorse di calcolare con precisione la disponibilità dei loro utenti e tenere conto del tempo che gli utenti dedicano al lavoro effettivo relativo al progetto, stiamo introducendo il concetto di orario di lavoro in Adobe Workfront.</p>
                        <p>È possibile definire il valore del campo Tempo di lavoro per ogni utente al momento della creazione o della modifica del profilo.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 16 febbraio 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Versione di produzione: 2 marzo 2023 (fuori ciclo)</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>


### Miglioramenti ai report e alle dashboard


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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-reports-dashboards.md" class="MCXref xref" xrefformat="{para}">Dashboard Canvas</a></p>
                        <p>I dashboard di Canvas sono stati aggiunti come funzionalità in corso di lavorazione per i dashboard che possono essere abilitati nei modelli di layout. I dashboard di Canvas consentono di combinare le visualizzazioni di Reporting Canvas con i rapporti esistenti, oltre a utilizzare nuove opzioni di layout. Attualmente sono supportati solo i rapporti elenco, ma verranno aggiunte più opzioni man mano che lo sviluppo continua.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Anteprima versione:N/D<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: con la versione 23.2</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}">Raccolte biometriche di accesso e bacheche nell’app mobile</span></a>
                        <p>L’accesso biometrico è ora un’opzione per accedere più rapidamente all’app mobile. Una volta impostata la verifica biometrica dopo il primo accesso, gli utenti potranno utilizzare il riconoscimento delle impronte digitali o del volto per accedere rapidamente di nuovo all’app e verificare solo occasionalmente la password. Inoltre, sono previsti diversi miglioramenti nell’esperienza di accesso generale, che verranno introdotti in un aggiornamento successivo.</p>
                        <p>Le raccolte di schede madri sono ora supportate anche nell’app mobile, consentendo agli utenti mobili di visualizzare dall’elenco delle schede madri qualsiasi raccolta a cui hanno accesso nella versione desktop.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Anteprima versione: N/D<br /></p>
                            </li>
                            <li>
                                 <p>Versione di produzione: disponibile in Apple App Store e Google Play Store il 13 marzo 2023</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nuovo su Workfront per i plug-in Creative Cloud</a>
                        <p>Abbiamo aggiunto le seguenti modifiche al Workfront per i plug-in Creative Cloud:
                        <ul>
                        <li>Il plug-in ora notifica quando un’attività ha un predecessore</li>
                        <li>Il coreano è ora una lingua supportata</li>
                        </ul> </p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Anteprima versione: N/D<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Versione di produzione: 23 marzo 2023 </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nuova esperienza di commento per i problemi Beta</a>
                        <p>È attualmente in fase di sviluppo un aggiornamento dell’esperienza di aggiunta di commenti in Adobe Workfront. Questo aggiornamento include una nuova interfaccia, nuove funzioni e prestazioni migliorate nella sezione Aggiornamenti di alcuni oggetti. </p>
                        <p>Questa nuova esperienza unificherà i commenti in Adobe Workfront e oltre, in Adobe Experience Cloud. </p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: 20 marzo 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Versione di produzione: con la versione 23.2 </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nuovi clienti da integrare in Adobe Unified Experience</a></p>
                        <p>L’esperienza unificata di Adobe include:
                        <ul>
                        <li>Un singolo accesso per tutte le applicazioni Adobe tramite Adobe Experience Cloud</li>
                        <li>Uno "switcher di organizzazione" per spostarsi tra le organizzazioni e gli ambienti Workfront</li>
                        <li>Navigazione con opzioni per pagine Workfront, preferenze Adobe Experience Cloud e il tuo profilo Workfront</li>
                        </ul>
                        </p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Anteprima versione: N/D<br /></p>
                            </li>
                            <li>
                                <p>Versione di produzione: metà-fine marzo 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Il visualizzatore di bozze si apre in una nuova scheda per gli utenti dell’esperienza unificata</a></p>
                        <p>Il visualizzatore di bozze ora si apre in una nuova scheda per gli utenti dell’esperienza unificata.
                        </p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Anteprima versione: N/D<br /></p>
                            </li>
                            <li>
                                <p>Versione di produzione: metà-fine marzo 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Esportare le tavole da disegno come file PDF singolo o più file PDF in Adobe Workfront per XD</span></a>
                        <p>Nel plug-in Adobe Workfront for XD, ora puoi scegliere di esportare le tavole da disegno come un singolo file PDF o più file PDF.</p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Anteprima versione: N/D<br /></p>
                            </li>
                            <li>
                                 <p>Versione di produzione: 6 febbraio 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-look-and-feel.md" class="MCXref xref" xrefformat="{para}">Aggiornamenti look-and-feel durante il periodo di rilascio della versione 23.2</a></p>
                        <p>Aggiornamenti minori al look and feel di varie aree dell’applicazione Adobe Workfront vengono effettuati entro l’intervallo di tempo della versione 23.2. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione almeno 2 settimane dopo il rilascio in anteprima. </p>
                    </td>
                    <td><p><b>Disponibile in queste date:</b></p>
                        <ul>
                            <li>
                                <p>Versione di anteprima: nell’arco temporale della versione 23.2<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Versione di produzione: almeno 2 settimane dopo il rilascio in anteprima (se non diversamente specificato)</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

## Notifiche

### Miglioramenti apportati a Workfront Fusion

Le nuove funzioni di Workfront Fusion sono disponibili in produzione a una cadenza al di fuori della pianificazione della versione 23.2. Per ulteriori informazioni sulle funzioni più recenti, consulta [Attività di rilascio di Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Miglioramenti di Workfront Scenario Planner

A questo punto della versione, non sono presenti aggiornamenti di Scenario Planner. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### Miglioramenti di Workfront Proof

A questo punto della versione, non sono presenti aggiornamenti di bozza per Workfront. Questa area verrà aggiornata quando saranno disponibili aggiornamenti.

### Miglioramenti agli obiettivi di Workfront

Nuove funzioni in arrivo nella versione Workfront Goals con la versione 23.2. Per informazioni su queste nuove funzioni ora disponibili in Anteprima, consulta [Obiettivi di Adobe Workfront con la versione 23.2](/help/quicksilver/product-announcements/product-releases/goals-release-activity/goals-23-2-release/goals-23-2-release.md).

### API versione 16

La versione 16 dell’API verrà rilasciata con la versione 22.3. Per API versione 16, abbiamo modificato alcune risorse ed endpoint. Alcune delle modifiche supportano nuove funzionalità, mentre altre semplificano l’utilizzo delle informazioni disponibili tramite l’API.

Per informazioni sulle novità e sugli aggiornamenti, consulta [Novità della versione 16 dell’API](/help/quicksilver/wf-api/api/new-api-version-16.md).

Per informazioni sulle versioni API, consulta [Pianificazione del supporto e del controllo delle versioni API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Aggiornamenti di manutenzione per Workfront

Per informazioni sugli aggiornamenti di manutenzione effettuati durante la versione 23.2, consulta [Aggiornamenti di manutenzione per Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Aggiornamenti dei corsi di formazione

Scopri gli ultimi aggiornamenti apportati a programmi di apprendimento, percorsi di apprendimento, video e guide per ogni versione di Adobe Workfront. Per ulteriori informazioni, consulta la sezione &quot;Novità&quot; del [Pagina Tutorials di Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).

### Funzionalità presto rimossa da Workfront

Le seguenti funzionalità verranno presto rimosse da Workfront:

#### **Le pagine esterne del dashboard non supportano più gli URL del dashboard**

Per migliorare la stabilità del dashboard e i tempi di caricamento, le pagine esterne nei dashboard non potranno più fare riferimento agli URL del dashboard. Gli amministratori di sistema per gli account che contengono pagine esterne che fanno riferimento a dashboard riceveranno una notifica in-app per avvisarli di questa modifica. Per ulteriori informazioni, consulta [Incorporare una pagina esterna in una dashboard](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

#### **Modifiche all’API predefinita di Workfront**

Per fare in modo che le chiamate API possano sfruttare le funzionalità API di Workfront più aggiornate, stiamo aggiornando l’API predefinita. Quando una chiamata API non specifica una versione dell’API, viene effettuata all’API predefinita.

Ora, l’API predefinita riflette la versione più recente dell’API. In futuro, aggiorneremo l’API predefinita ogni volta che viene rilasciata una nuova versione dell’API, in modo che le chiamate all’API predefinita utilizzino sempre la versione più recente.

In precedenza, l’API predefinita utilizzava la versione 2.0 dell’API di Workfront, che è stata dichiarata obsoleta.

Se l’organizzazione utilizza attualmente l’API predefinita obsoleta, l’amministratore di Workfront ha ricevuto un messaggio del Centro notifiche con ulteriori istruzioni relative all’API predefinita.

Per ulteriori informazioni, consulta [Aggiornare le integrazioni che utilizzano il controllo delle versioni API predefinito](/help/quicksilver/wf-api/api/update-default-api-versioning.md).


<!--
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

        -->
