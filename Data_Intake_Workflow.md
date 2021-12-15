# Media Delivery Workflows

##  Partners delivering their own media to dev team
![image](https://mermaid.ink/img/eyJjb2RlIjoiZ3JhcGggVERcblxuJSUlIE5PREUgREVGSU5JVElPTlNcblxuJSUgbWVkaWEgaW50YWtlIG5vZGVcbmlkMXtzdGFrZWhvbGRlciBlbWFpbHMgTWF4IDxicj4gdG8gcmVxdWVzdCBtZWRpYX1cblxuJSUgc3Vibm9kZXMgZm9yIG1lZGlhIHR5cGVzXG5pZDEuMShNYXggZmluZHMgbWVkaWEgd2hpY2ggPGJyPiBtYXRjaGVzIHRoZSByZXF1ZXN0KVxuaWQxLjIoTWF4IGRvZXMgbm90IGZpbmQgbWF0Y2hpbmcgbWVkaWEpXG5cbiUlIG1lZGlhIGRlc3RpbmF0aW9uIDAxXG5pZDJbTWF4IHNlbmRzIGFjY2VzcyBjb3BpZXMgb2YgdGhlIDxicj4gbWVkaWEgdG8gY29uZmlybSB0aGF0IGl0IG1hdGNoZXMgPGJyPiB0aGUgc3Rha2Vob2xkZXIncyByZXF1ZXN0XVxuaWQyLjF7TWF4IGFwb2xhZ2V0aWNhbGx5IDxicj4gZW1haWxzIHN0YWtlaG9sZGVyfVxuaWQyLjJbc3Rha2Vob2xkZXIgYXBwcm92ZXMgc3BlY2lmaWMgZmlsZXNdXG5pZDIuM1tzdGFrZWhvbGRlciBkb2VzIG5vdCBhcHByb3ZlIGFueSBmaWxlc11cbmlkMi40W01heCBmaWxlcyBhcHByb3ByaWF0ZSA8YnI-IHBhcGVyd29yayBmb3IgcHVibGljYXRpb25dXG5cbiUlIGNvbmNsdXNpb25cbmlkNHtNYXggZmlsZXMgYXNzZXRzIGluIHRoZSA8YnI-IGFwcHJvcHJpYXRlIHByb2plY3QgPGJyPiBmb2xkZXJzLn1cblxuJSUgZGlhZ3JhbVxuaWQxIC0tPiBpZDEuMSAmIGlkMS4yXG5pZDEuMSAtLT4gaWQyIC0tPiBpZDIuMiAmIGlkMi4zIFxuaWQxLjIgLS0-IGlkMi4xXG5pZDIuMiAtLT4gaWQyLjRcbmlkMi4zIC0tPiBpZDIuMVxuaWQyLjQgLS0-IGlkNFxuIiwibWVybWFpZCI6eyJ0aGVtZSI6ImRlZmF1bHQifSwidXBkYXRlRWRpdG9yIjpmYWxzZSwiYXV0b1N5bmMiOnRydWUsInVwZGF0ZURpYWdyYW0iOmZhbHNlfQ)
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

