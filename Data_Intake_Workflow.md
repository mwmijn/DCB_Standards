# Media Delivery Workflows

##  Partners delivering their own media to dev team
<div class="mermaid">
graph TD

%%% NODE DEFINITIONS

%% media intake node
id1{incoming media}

%% subnodes for media types
id1.1(images)
id1.2(video)
id1.3(text)

%% media destination 01
id2[upload files to <br/> appbox
id2.1[email as attachment to Max]
id2.2[email Max to tell them what the file is]

%% consent
id3[Max replies to confirm receipt <br> and file metadata as well <br>  as to request formal consent <br> to archive and share data]

%% conclusion
id4{partner returns <br> signed consent form <br> and Max files assets in the <br> appropriate project <br> folders}
%% diagram
id1 --> id1.1 & id1.3 & id1.2
id1.1 & id1.2 --> id2 --> id2.2
id1.3 --> id2.1
id2.1 & id2.2 --> id3
id3 --> id4
</div>

<br>

--- 

# Partners requesting media from ASM
``` mermaid
graph TD

%%% NODE DEFINITIONS

%% media intake node
id1{partner emails Max <br> to request media}

%% subnodes for media types
id1.1(Max finds media which <br> matches the request)
id1.2(Max does not find matching media)
id1.3(request is general/returns far too many results)

%% media destination 01
id2[Max sends access copies of the <br> media to confirm that it matches <br> the partner's request]
id2.1{Max apolagetically <br> emails partner}
id2.2[partner approves specific files]
id2.3[partner does not approve any files]
id2.4[Max files appropriate <br> paperwork for publication]
id2.5[Max schedules in-person search with partner at museum]

%% In person search details
id3.1(partner approves some media)

%% conclusion
id4{Max files assets in the <br> appropriate project <br> folders}

%% diagram
id1 --> id1.1 & id1.2 & id1.3
id1.1 --> id2 --> id2.2 & id2.3 
id1.2 --> id2.1
id1.3 --> id2.5
id2.2 --> id2.4
id2.3 --> id2.1
id2.4 --> id4
id2.5 --> id3.1 --> id2.4
```
<br>

--- 

# General Post-Intake Workflow
```mermaid
graph TD

%% first set of nodes
id1.1{media from <br> ASM collection}
id1.2{media that <br> partner owns <br> digitized by Max}
id1.3{media created <br> for the project <br> such as VVC or 3D}

%% second set of nodes, step one of intake process
id2.1(archive copy duplicated to /media/archive)
id2.2(original archive copy stored in /media/archive)

%% third set of nodes, creating access and asset copies
id3.1[AB used to create jpeg access <br> copies incl. stills of VVC and 3D, <br> renamed appropriately <br> stored in /media/access <br> <br> necessary asset copies are <br> created, renamed appropriately <br> and stored in /media/assets]

%% Chart
id1.1 --> id2.1
id1.2 & id1.3 --> id2.2

id2.1 & id2.2 --> id3.1 
```
<br>

---

