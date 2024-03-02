[//]: # (auto_md_to_doc_comments segment start A)

# dropbox_backup_to_external_disk_2

[//]: # (auto_cargo_toml_to_md start)

**TUI, GUI, CLI and LIB, one way sync from dropbox to external disc**  
***version: 2023.820.1613 date: 2023-08-20 author: [bestia.dev](https://bestia.dev) repository: [Github](https://github.com/bestia-dev/dropbox_backup_to_external_disk_2/)***  

[//]: # (auto_cargo_toml_to_md end)

 ![maintained](https://img.shields.io/badge/maintained-green)
 ![work_in_progress](https://img.shields.io/badge/work_in_progress-yellow)


 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/bestia-dev/dropbox_backup_to_external_disk_2/blob/main/LICENSE)
 ![Hits](https://bestia.dev/webpage_hit_counter/get_svg_image/804435805.svg)

Hashtags: #rustlang #tutorial #dropbox #cli #tui  
My projects on Github are more like a tutorial than a finished product: [bestia-dev tutorials](https://github.com/bestia-dev/tutorials_rust_wasm).

## Version 2

The second version will have separated projects for [CLI](https://github.com/bestia-dev/dropbox_backup_to_external_disk_cli), [TUI](https://github.com/bestia-dev/dropbox_backup_to_external_disk_tui) and [GUI](https://github.com/bestia-dev/dropbox_backup_to_external_disk_gui) interfaces with a common [LIB](https://github.com/bestia-dev/dropbox_backup_to_external_disk_lib) project.  
This is to show how the same library can be used from different user-interfaces.  
In Cargo.toml I can use the local path to define the dependency and that way I have always the newest code available:

```toml
[dependencies]
dropbox_backup_to_external_disk_lib = { path = "../dropbox_backup_to_external_disk_lib" }
```

VSCode is so smart that for `Go to definition` it even opens the file from the library, so I can modify that. For editing it feels just like one project.  

The prototype CLI where I experimented with the Dropbox api is here: [dropbox_backup_to_external_disk_1](https://github.com/bestia-dev/dropbox_backup_to_external_disk_1).  

## Development

From inside the development container I need to have access to the external disk directory where the dropbox backup is and access to the dropbox.com.  
I wrote a new bash script `rust_dev_pod_create.sh` to create a podman pod for this project and named it "pod_with_rust_vscode_for_dropbox".

## Open-source and free as a beer

My open-source projects are free as a beer (MIT license).  
I just love programming.  
But I need also to drink. If you find my projects and tutorials helpful, please buy me a beer by donating to my [PayPal](https://paypal.me/LucianoBestia).  
You know the price of a beer in your local bar ;-)  
So I can drink a free beer for your health :-)  
[Na zdravje!](https://translate.google.com/?hl=en&sl=sl&tl=en&text=Na%20zdravje&op=translate) [Alla salute!](https://dictionary.cambridge.org/dictionary/italian-english/alla-salute) [Prost!](https://dictionary.cambridge.org/dictionary/german-english/prost) [Nazdravlje!](https://matadornetwork.com/nights/how-to-say-cheers-in-50-languages/) 🍻

[//bestia.dev](https://bestia.dev)  
[//github.com/bestia-dev](https://github.com/bestia-dev)  
[//bestiadev.substack.com](https://bestiadev.substack.com)  
[//youtube.com/@bestia-dev-tutorials](https://youtube.com/@bestia-dev-tutorials)  

[//]: # (auto_md_to_doc_comments segment end A)
