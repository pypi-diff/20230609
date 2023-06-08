# Comparing `tmp/pywry-0.5.8.tar.gz` & `tmp/pywry-0.5.9.tar.gz`

## Comparing `pywry-0.5.8.tar` & `pywry-0.5.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 pywry-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 pywry-0.5.8/rust_src/pywry/Cargo.toml
--rw-r--r--   0     1001      123     1063 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/LICENSE
--rw-r--r--   0     1001      123     4924 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/README.md
--rw-r--r--   0     1001      123     3565 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/constants.rs
--rw-r--r--   0     1001      123     6202 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/events.rs
--rw-r--r--   0     1001      123     3733 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/handlers.rs
--rw-r--r--   0     1001      123     5780 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/headless.rs
--rw-r--r--   0     1001      123     1571 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/lib.rs
--rw-r--r--   0     1001      123      975 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/pipe.rs
--rw-r--r--   0     1001      123     7516 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/structs.rs
--rw-r--r--   0     1001      123     1366 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/utils.rs
--rw-r--r--   0     1001      123     6168 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/window.rs
--rw-r--r--   0     1001      123    63815 2023-05-15 22:14:50.000000 pywry-0.5.8/Cargo.lock
--rw-r--r--   0     1001      123     1155 2023-05-15 22:14:50.000000 pywry-0.5.8/python/pywry/backend.py
--rw-r--r--   0     1001      123        0 2023-05-15 22:14:50.000000 pywry-0.5.8/python/pywry/py.typed
--rw-r--r--   0     1001      123      180 2023-05-15 22:14:50.000000 pywry-0.5.8/python/pywry/__init__.py
--rw-r--r--   0     1001      123    14443 2023-05-15 22:14:50.000000 pywry-0.5.8/python/pywry/core.py
--rw-r--r--   0     1001      123      217 2023-05-15 22:14:50.000000 pywry-0.5.8/python/pywry/pywry.pyi
--rw-r--r--   0     1001      123      733 2023-05-15 22:14:50.000000 pywry-0.5.8/Cargo.toml
--rw-r--r--   0     1001      123     3565 2023-05-15 22:14:50.000000 pywry-0.5.8/src/constants.rs
--rw-r--r--   0     1001      123     6202 2023-05-15 22:14:50.000000 pywry-0.5.8/src/events.rs
--rw-r--r--   0     1001      123     3733 2023-05-15 22:14:50.000000 pywry-0.5.8/src/handlers.rs
--rw-r--r--   0     1001      123     5780 2023-05-15 22:14:50.000000 pywry-0.5.8/src/headless.rs
--rw-r--r--   0     1001      123     1571 2023-05-15 22:14:50.000000 pywry-0.5.8/src/lib.rs
--rw-r--r--   0     1001      123      975 2023-05-15 22:14:50.000000 pywry-0.5.8/src/pipe.rs
--rw-r--r--   0     1001      123     7516 2023-05-15 22:14:50.000000 pywry-0.5.8/src/structs.rs
--rw-r--r--   0     1001      123     1366 2023-05-15 22:14:50.000000 pywry-0.5.8/src/utils.rs
--rw-r--r--   0     1001      123     6168 2023-05-15 22:14:50.000000 pywry-0.5.8/src/window.rs
--rw-r--r--   0        0        0     5526 1970-01-01 00:00:00.000000 pywry-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 pywry-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pywry-0.5.9/rust_src/pywry/Cargo.toml
+-rw-r--r--   0     1001      123     1063 2023-05-25 16:44:14.000000 pywry-0.5.9/rust_src/pywry/LICENSE
+-rw-r--r--   0     1001      123     5351 2023-05-25 16:44:14.000000 pywry-0.5.9/rust_src/pywry/README.md
+-rw-r--r--   0     1001      123     3565 2023-05-25 16:44:14.000000 pywry-0.5.9/rust_src/pywry/src/constants.rs
+-rw-r--r--   0     1001      123     6151 2023-05-25 16:44:14.000000 pywry-0.5.9/rust_src/pywry/src/events.rs
+-rw-r--r--   0     1001      123     3697 2023-05-25 16:44:14.000000 pywry-0.5.9/rust_src/pywry/src/handlers.rs
+-rw-r--r--   0     1001      123     5780 2023-05-25 16:44:14.000000 pywry-0.5.9/rust_src/pywry/src/headless.rs
+-rw-r--r--   0     1001      123     1571 2023-05-25 16:44:14.000000 pywry-0.5.9/rust_src/pywry/src/lib.rs
+-rw-r--r--   0     1001      123      975 2023-05-25 16:44:14.000000 pywry-0.5.9/rust_src/pywry/src/pipe.rs
+-rw-r--r--   0     1001      123     8680 2023-05-25 16:44:14.000000 pywry-0.5.9/rust_src/pywry/src/structs.rs
+-rw-r--r--   0     1001      123     1366 2023-05-25 16:44:14.000000 pywry-0.5.9/rust_src/pywry/src/utils.rs
+-rw-r--r--   0     1001      123     6984 2023-05-25 16:44:14.000000 pywry-0.5.9/rust_src/pywry/src/window.rs
+-rw-r--r--   0     1001      123    63830 2023-05-25 16:44:14.000000 pywry-0.5.9/Cargo.lock
+-rw-r--r--   0     1001      123     1155 2023-05-25 16:44:14.000000 pywry-0.5.9/python/pywry/backend.py
+-rw-r--r--   0     1001      123        0 2023-05-25 16:44:14.000000 pywry-0.5.9/python/pywry/py.typed
+-rw-r--r--   0     1001      123      180 2023-05-25 16:44:14.000000 pywry-0.5.9/python/pywry/__init__.py
+-rw-r--r--   0     1001      123    14493 2023-05-25 16:44:14.000000 pywry-0.5.9/python/pywry/core.py
+-rw-r--r--   0     1001      123      217 2023-05-25 16:44:14.000000 pywry-0.5.9/python/pywry/pywry.pyi
+-rw-r--r--   0     1001      123      749 2023-05-25 16:44:14.000000 pywry-0.5.9/Cargo.toml
+-rw-r--r--   0     1001      123     3565 2023-05-25 16:44:14.000000 pywry-0.5.9/src/constants.rs
+-rw-r--r--   0     1001      123     6151 2023-05-25 16:44:14.000000 pywry-0.5.9/src/events.rs
+-rw-r--r--   0     1001      123     3697 2023-05-25 16:44:14.000000 pywry-0.5.9/src/handlers.rs
+-rw-r--r--   0     1001      123     5780 2023-05-25 16:44:14.000000 pywry-0.5.9/src/headless.rs
+-rw-r--r--   0     1001      123     1571 2023-05-25 16:44:14.000000 pywry-0.5.9/src/lib.rs
+-rw-r--r--   0     1001      123      975 2023-05-25 16:44:14.000000 pywry-0.5.9/src/pipe.rs
+-rw-r--r--   0     1001      123     8680 2023-05-25 16:44:14.000000 pywry-0.5.9/src/structs.rs
+-rw-r--r--   0     1001      123     1366 2023-05-25 16:44:14.000000 pywry-0.5.9/src/utils.rs
+-rw-r--r--   0     1001      123     6984 2023-05-25 16:44:14.000000 pywry-0.5.9/src/window.rs
+-rw-r--r--   0        0        0     5953 1970-01-01 00:00:00.000000 pywry-0.5.9/PKG-INFO
```

### Comparing `pywry-0.5.8/pyproject.toml` & `pywry-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pywry"
-version = "0.5.8"
+version = "0.5.9"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: POSIX",
     "Operating System :: Microsoft :: Windows",
```

### Comparing `pywry-0.5.8/rust_src/pywry/Cargo.toml` & `pywry-0.5.9/rust_src/pywry/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.8"
+version = "0.5.9"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
@@ -21,7 +21,8 @@
 image = { version = "^0.24.5", default-features = false, features = ["png"] }
 tokio = { version = "^1.23.0", features = ["rt", "rt-multi-thread", "full"] }
 serde = { version = "^1.0", features = ["derive"] }
 serde_json = "^1.0"
 mime_guess = "^2.0"
 urlencoding = "^2.1.2"
 open = "^4.0"
+rand = "^0.8.4"
```

### Comparing `pywry-0.5.8/rust_src/pywry/LICENSE` & `pywry-0.5.9/rust_src/pywry/LICENSE`

 * *Files identical despite different names*

### Comparing `pywry-0.5.8/rust_src/pywry/README.md` & `pywry-0.5.9/rust_src/pywry/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -153,7 +153,11 @@
 ---------------------
 
 ### Troubleshooting Linux
 
 #### `"/lib/x86_64-linux-gnu/libgio-2.0.so.0: undefined symbol: g_module_open_full"`
 
 This is a known issue with the `gio` library. You can fix it by installing the `libglib2.0-dev` package.
+
+
+
+PyWry is a project that aims to provide Python bindings for WRY, a cross-platform webview library. WRY is a trademark of the Tauri Program within the Commons Conservancy and PyWry is not officially endorsed or supported by them. PyWry is an independent and community-driven effort that respects the original goals and values of Tauri and WRY. PyWry does not claim any ownership or affiliation with WRY or the Tauri Program.
```

### Comparing `pywry-0.5.8/rust_src/pywry/src/constants.rs` & `pywry-0.5.9/rust_src/pywry/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.8/rust_src/pywry/src/events.rs` & `pywry-0.5.9/rust_src/pywry/src/events.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-use crate::{
-	structs::{ConsolePrinter, PlotData, UserEvent},
-};
+use crate::structs::{ConsolePrinter, PlotData, UserEvent};
 
 #[cfg(not(target_os = "macos"))]
 use crate::utils::decode_path;
 
 use std::{
 	collections::HashMap,
 	io::{self, Write},
@@ -50,15 +48,14 @@
 					)
 					.unwrap();
 				handler.flush().unwrap();
 			});
 		}
 		// UserEvent::NewPlot
 		Event::UserEvent(UserEvent::NewPlot(data, _windowid)) => {
-			let _proxy = proxy.clone();
 			let plot_data = PlotData::to_json(&data).to_string();
 
 			webviews
 				.iter_mut()
 				.next()
 				.unwrap()
 				.1
@@ -75,29 +72,29 @@
 				None => {}
 			}
 		}
 		// UserEvent::DownloadStarted
 		#[cfg(not(target_os = "macos"))]
 		Event::UserEvent(UserEvent::DownloadStarted(uri, path)) => {
 			if uri.len() < 200 {
-				console.debug(&format!("\nDownload Started: {}", uri));
+				console.debug(&format!("Download Started: {}", uri));
 			}
-			console.debug(&format!("\nPath: {}", path));
+			console.debug(&format!("Path: {}", path));
 		}
 		// UserEvent::DownloadComplete
 		#[cfg(not(target_os = "macos"))]
 		Event::UserEvent(UserEvent::DownloadComplete(
 			filepath,
 			success,
 			download_path,
 			export_image,
 			window_id,
 		)) => {
 			let is_export = !export_image.is_empty();
-			console.debug(&format!("\nDownload Complete: {}", success));
+			console.debug(&format!("Download Complete: {}", success));
 
 			let decoded = decode_path(&filepath.unwrap().to_str().unwrap());
 
 			let new_path = match !download_path.is_empty() {
 				true => match !export_image.is_empty() {
 					true => {
 						let path = PathBuf::from(&export_image);
@@ -109,30 +106,30 @@
 						path.to_path_buf()
 					}
 				},
 
 				false => decoded.to_path_buf(),
 			};
 
-			console.debug(&format!("\nOriginal Path: {:?}", decoded));
+			console.debug(&format!("Original Path: {:?}", decoded));
 			console.debug(&format!("New Path: {:?}", new_path));
 
 			let dir = new_path.parent().unwrap();
 			match !dir.exists() {
 				true => {
-					console.debug(&format!("\nCreating directory: {:?}", dir));
+					console.debug(&format!("Creating directory: {:?}", dir));
 					if let Err(error) = create_dir_all(dir) {
 						console.error(&format!("Error creating directory: {}", error));
 					}
 				}
 				false => {}
 			}
 
 			match copy(&decoded, &new_path) {
-				Err(error) => console.error(&format!("\nError copying file: {}", error)),
+				Err(error) => console.error(&format!("Error copying file: {}", error)),
 				Ok(_) => {
 					if is_export {
 						proxy.send_event(UserEvent::CloseWindow(window_id)).unwrap_or_default();
 					}
 					if let Err(error) = remove_file(&decoded) {
 						console.error(&format!("Error deleting file: {}", error));
 					}
@@ -186,15 +183,15 @@
 					console.error(&format!("Error opening file: {}", error));
 				}
 			}
 		}
 		// WindowEvent::NewWindow
 		#[cfg(not(target_os = "windows"))]
 		Event::UserEvent(UserEvent::NewWindow(uri, window_icon)) => {
-			console.debug(&format!("\nNew Window Requested: {}", uri));
+			console.debug(&format!("New Window Requested: {}", uri));
 			match uri.starts_with("http://") || uri.starts_with("https://") {
 				true => {
 					let pre_window = WindowBuilder::new()
 						.with_title(uri.to_string())
 						.with_window_icon(window_icon)
 						.with_inner_size(LogicalSize::new(1300, 900))
 						.with_resizable(true)
```

### Comparing `pywry-0.5.8/rust_src/pywry/src/handlers.rs` & `pywry-0.5.9/rust_src/pywry/src/handlers.rs`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,17 @@
 				}
 			}
 		})
 		.with_ipc_handler({
 			let proxy = proxy.clone();
 			move |_, string| match string.as_str() {
 				_ if string.starts_with("#PYWRY_RESULT:") => {
-					let result = string.replace("#PYWRY_RESULT:", "").to_string();
-					proxy.send_event(UserEvent::STDout(result)).unwrap_or_default();
+					proxy
+						.send_event(UserEvent::STDout(string[14..].to_string()))
+						.unwrap_or_default();
 
 					if !is_headless {
 						proxy.send_event(UserEvent::CloseWindow(window_id)).unwrap_or_default();
 					}
 				}
 				_ if string.starts_with("data:") => {
 					proxy.send_event(UserEvent::BlobChunk(Some(string))).unwrap_or_default();
```

### Comparing `pywry-0.5.8/rust_src/pywry/src/headless.rs` & `pywry-0.5.9/rust_src/pywry/src/headless.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.8/rust_src/pywry/src/lib.rs` & `pywry-0.5.9/rust_src/pywry/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.8/rust_src/pywry/src/pipe.rs` & `pywry-0.5.9/rust_src/pywry/src/pipe.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.8/rust_src/pywry/src/structs.rs` & `pywry-0.5.9/rust_src/pywry/src/structs.rs`

 * *Files 8% similar despite different names*

```diff
@@ -100,24 +100,57 @@
 	NewPlot(String, WindowId),
 	OpenFile(Option<PathBuf>),
 	STDout(String),
 	#[cfg(not(target_os = "windows"))]
 	NewWindow(String, Option<Icon>),
 }
 
+pub struct WebViewOptions {
+	/// URL to be loaded when the webview is ready.
+	pub url: String,
+	/// JavaScript code to be injected when the webview is ready.
+	pub init_script: Option<String>,
+}
+
+impl Default for WebViewOptions {
+	/// Returns a default set of WebViewOptions.
+	fn default() -> Self {
+		Self { url: "wry://localhost".to_string(), init_script: None }
+	}
+}
+
+impl WebViewOptions {
+	pub fn new() -> Self {
+		Self::default()
+	}
+
+	/// Sets the URL to be loaded when the webview is ready.
+	pub fn with_url(mut self, url: String) -> Self {
+		self.url = url;
+		self
+	}
+
+	/// Sets the JavaScript code to be injected when the webview is ready.
+	pub fn with_init_script(mut self, init_script: String) -> Self {
+		self.init_script = Some(init_script);
+		self
+	}
+}
+
 pub struct Showable {
 	pub content: String,
 	pub title: String,
 	pub height: Option<u32>,
 	pub width: Option<u32>,
 	pub icon: String,
 	pub data: Option<Value>,
 	pub download_path: String,
 	pub export_image: String,
 	pub theme: Theme,
+	pub options: WebViewOptions,
 }
 
 impl Showable {
 	pub fn new(raw_json: &str) -> Option<Self> {
 		match Self::from_json(raw_json) {
 			Some(item) => Some(item),
 			None => Some(Self::default()),
@@ -145,27 +178,35 @@
 		let icon = json["icon"].as_str().unwrap_or_default().to_string();
 		let title = json["title"].as_str().unwrap_or_default().to_string();
 		let mut height: Option<u32> =
 			json["height"].as_u64().and_then(|x| u32::try_from(x).ok());
 		let mut width: Option<u32> =
 			json["width"].as_u64().and_then(|x| u32::try_from(x).ok());
 		let mut theme = Theme::Light;
+		let mut options = WebViewOptions::new();
 
 		if !json_data.is_null() {
 			theme = match json_data["theme"].as_str().unwrap_or_default() {
 				"dark" => Theme::Dark,
 				"light" => Theme::Light,
 				_ => theme,
 			};
 			if json_data["layout"].is_object() {
 				let raw_width = json_data["layout"]["width"].as_u64().unwrap_or(800);
 				let raw_height = json_data["layout"]["height"].as_u64().unwrap_or(600);
 				width = Some(u32::try_from(raw_width).unwrap_or(800));
 				height = Some(u32::try_from(raw_height).unwrap_or(600));
 			}
+			if json_data["url"].is_string() {
+				options = options.with_url(json_data["url"].as_str().unwrap().to_string());
+			}
+			if json_data["init_script"].is_string() {
+				options = options
+					.with_init_script(json_data["init_script"].as_str().unwrap().to_string());
+			}
 		}
 
 		let export_image = json["export_image"].as_str().unwrap_or_default().to_string();
 		let download_path = json["download_path"].as_str().unwrap_or_default().to_string();
 
 		Some(Self {
 			content,
@@ -173,14 +214,15 @@
 			height,
 			width,
 			icon,
 			data: Some(json_data),
 			download_path,
 			export_image,
 			theme,
+			options,
 		})
 	}
 }
 
 impl Default for Showable {
 	fn default() -> Self {
 		Self {
@@ -193,14 +235,15 @@
 			height: None,
 			width: None,
 			icon: "".to_string(),
 			data: None,
 			download_path: "".to_string(),
 			export_image: "".to_string(),
 			theme: Theme::Light,
+			options: WebViewOptions::default(),
 		}
 	}
 }
 
 pub struct ShowableHeadless {
 	pub data: Option<Value>,
 	pub export_image: String,
```

### Comparing `pywry-0.5.8/rust_src/pywry/src/utils.rs` & `pywry-0.5.9/rust_src/pywry/src/utils.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.8/rust_src/pywry/src/window.rs` & `pywry-0.5.9/rust_src/pywry/src/window.rs`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	collections::HashMap,
 	fs::{canonicalize, read},
 	sync::mpsc::{Receiver, Sender},
 };
 
 use wry::{
 	application::{
-		dpi::LogicalSize,
+		dpi::{LogicalSize, PhysicalPosition},
 		event_loop::{ControlFlow, EventLoop, EventLoopProxy, EventLoopWindowTarget},
 		window::{Theme, WindowBuilder, WindowId},
 	},
 	http::{header::CONTENT_TYPE, Response},
 	webview::{WebView, WebViewBuilder},
 };
 
@@ -43,16 +43,26 @@
 			let mut dev_tools_html = DEV_TOOLS_HTML.as_bytes().to_vec();
 			dev_tools_html.extend(content);
 			dev_tools_html
 		}
 		false => content,
 	};
 
+	let json_data = to_show.data.clone().unwrap_or_default();
+	console.debug(&format!("json_data: {}", json_data));
+
+	let screen_size = event_loop.available_monitors().nth(0).unwrap().size();
+	let window_size = (to_show.width.unwrap_or(800), to_show.height.unwrap_or(600));
+
 	let mut pre_window = WindowBuilder::new()
 		.with_title(to_show.title)
+		.with_position(PhysicalPosition::new(
+			(screen_size.width / 2) - (window_size.0 / 2) + (rand::random::<u32>() % 100),
+			(screen_size.height / 2) - (window_size.1 / 2) + (rand::random::<u32>() % 100),
+		))
 		.with_window_icon(get_icon(&window_icon))
 		.with_min_inner_size(LogicalSize::new(800, 450))
 		.with_theme(Some(Theme::Dark));
 
 	if to_show.height.is_some() && to_show.width.is_some() {
 		pre_window = pre_window.with_inner_size(LogicalSize::new(
 			to_show.width.unwrap_or(800) + 80,
@@ -61,15 +71,15 @@
 	}
 
 	let window = match pre_window.build(event_loop) {
 		Err(error) => return Err(error.to_string()),
 		Ok(item) => item,
 	};
 
-	let minimized = !to_show.export_image.is_empty();
+	let minimized = !to_show.export_image.is_empty() && !console.active;
 	if minimized {
 		window.set_visible(false);
 		window.set_maximized(false);
 	} else {
 		window.set_always_on_top(true);
 	}
 
@@ -80,18 +90,19 @@
 		_ => (255, 255, 255, 255),
 	};
 
 	let webview = match WebViewBuilder::new(window) {
 		Err(error2) => return Err(error2.to_string()),
 		Ok(item) => item,
 	};
-	let protocol = webview
-		.with_background_color(background_color)
-		.with_hotkeys_zoom(true)
-		.with_custom_protocol("wry".into(), move |request| {
+	let protocol =
+		webview.with_background_color(background_color).with_hotkeys_zoom(true);
+
+	let protocol = match to_show.options.url.starts_with("wry://") {
+		true => protocol.with_custom_protocol("wry".into(), move |request| {
 			let path = request.uri().path();
 			let clean_path = &path[1..];
 			let content = content.clone();
 			let mut mime = mime_guess::from_path("index.html");
 
 			let content = if path == "/" {
 				content.into()
@@ -110,15 +121,18 @@
 				.unwrap_or_else(|| "text/plain".to_string());
 
 			Response::builder()
 				.header(CONTENT_TYPE, mimetype)
 				.header("Access-Control-Allow-Origin", "null")
 				.body(content)
 				.map_err(Into::into)
-		});
+		}),
+		false => protocol,
+	};
+
 	let export_image = to_show.export_image.clone();
 	let _is_export = !export_image.is_empty();
 	let download_path = to_show.download_path.clone();
 
 	let init_view = match !to_show.data.is_none() {
 		true => {
 			let variable_value =
@@ -145,15 +159,20 @@
 		window_id,
 		download_path,
 		export_image,
 		&window_icon,
 		Some(false),
 	);
 
-	return match init_view.with_devtools(console.active).with_url("wry://localhost") {
+	let init_view = match to_show.options.init_script.is_some() {
+		true => init_view.with_initialization_script(&to_show.options.init_script.unwrap()),
+		false => init_view,
+	};
+
+	return match init_view.with_devtools(console.active).with_url(&to_show.options.url) {
 		Err(error3) => return Err(error3.to_string()),
 		Ok(subitem) => match subitem.build() {
 			Err(error4) => return Err(error4.to_string()),
 			Ok(sub2item) => {
 				if !minimized {
 					let proxy = proxy.clone();
 					proxy.send_event(UserEvent::NewWindowCreated(window_id)).unwrap_or_default();
@@ -189,15 +208,15 @@
 
 	event_loop.run(move |event, event_loop, control_flow| {
 		*control_flow = ControlFlow::Poll;
 
 		let response = receiver.try_recv().unwrap_or_default();
 
 		if !response.is_empty() {
-			console.debug("\nReceived response");
+			console.debug("Received message from Python");
 
 			let chart = Showable::new(&response).unwrap_or_default();
 			match create_new_window(chart, &event_loop, &proxy, console) {
 				Err(error) => console.error(&format!("Error creating window: {}", error)),
 				Ok(new_window) => {
 					webviews.insert(new_window.0, new_window.1);
 				}
```

### Comparing `pywry-0.5.8/Cargo.lock` & `pywry-0.5.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1513,20 +1513,21 @@
 checksum = "a915bd72824962bf190bbd3e8a044cccb695d1409f73ff5493712eda5136c7a8"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pywry"
-version = "0.5.8"
+version = "0.5.9"
 dependencies = [
  "image",
  "mime_guess",
  "open",
  "pyo3",
+ "rand 0.8.5",
  "serde",
  "serde_json",
  "tokio",
  "urlencoding",
  "wry",
 ]
```

### Comparing `pywry-0.5.8/python/pywry/backend.py` & `pywry-0.5.9/python/pywry/backend.py`

 * *Files identical despite different names*

### Comparing `pywry-0.5.8/python/pywry/core.py` & `pywry-0.5.9/python/pywry/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,26 +329,27 @@
         try:
             if self.init_engine:
                 # if there is data in the init_engine list,
                 # we send it to the backend and clear the list
                 for msg in self.init_engine:
                     self.runner.stdin.write(f"{msg}\n".encode())
                     await self.runner.stdin.drain()
-                self.init_engine = []
+                self.init_engine.clear()
 
             while self._is_started.is_set():
                 try:
                     if self.outgoing:
                         data = self.outgoing.pop(0)
                         with self.lock:
                             self.init_engine.append(data)
                         self.runner.stdin.write(f"{data}\n".encode())
                         await self.runner.stdin.drain()
 
-                        self.init_engine = []
+                        with self.lock:
+                            self.init_engine.clear()
 
                     await asyncio.sleep(0.5)
 
                 except (BrokenPipeError, ConnectionResetError) as pipe_err:
                     await self.exception_handler(pipe_err)
                     await self.run_backend()
```

### Comparing `pywry-0.5.8/Cargo.toml` & `pywry-0.5.9/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.8"
+version = "0.5.9"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
@@ -21,7 +21,8 @@
 image = { version = "^0.24.5", default-features = false, features = ["png"] }
 tokio = { version = "^1.23.0", features = ["rt", "rt-multi-thread", "full"] }
 serde = { version = "^1.0", features = ["derive"] }
 serde_json = "^1.0"
 mime_guess = "^2.0"
 urlencoding = "^2.1.2"
 open = "^4.0"
+rand = "^0.8.4"
```

### Comparing `pywry-0.5.8/src/constants.rs` & `pywry-0.5.9/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.8/src/events.rs` & `pywry-0.5.9/src/events.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-use crate::{
-	structs::{ConsolePrinter, PlotData, UserEvent},
-};
+use crate::structs::{ConsolePrinter, PlotData, UserEvent};
 
 #[cfg(not(target_os = "macos"))]
 use crate::utils::decode_path;
 
 use std::{
 	collections::HashMap,
 	io::{self, Write},
@@ -50,15 +48,14 @@
 					)
 					.unwrap();
 				handler.flush().unwrap();
 			});
 		}
 		// UserEvent::NewPlot
 		Event::UserEvent(UserEvent::NewPlot(data, _windowid)) => {
-			let _proxy = proxy.clone();
 			let plot_data = PlotData::to_json(&data).to_string();
 
 			webviews
 				.iter_mut()
 				.next()
 				.unwrap()
 				.1
@@ -75,29 +72,29 @@
 				None => {}
 			}
 		}
 		// UserEvent::DownloadStarted
 		#[cfg(not(target_os = "macos"))]
 		Event::UserEvent(UserEvent::DownloadStarted(uri, path)) => {
 			if uri.len() < 200 {
-				console.debug(&format!("\nDownload Started: {}", uri));
+				console.debug(&format!("Download Started: {}", uri));
 			}
-			console.debug(&format!("\nPath: {}", path));
+			console.debug(&format!("Path: {}", path));
 		}
 		// UserEvent::DownloadComplete
 		#[cfg(not(target_os = "macos"))]
 		Event::UserEvent(UserEvent::DownloadComplete(
 			filepath,
 			success,
 			download_path,
 			export_image,
 			window_id,
 		)) => {
 			let is_export = !export_image.is_empty();
-			console.debug(&format!("\nDownload Complete: {}", success));
+			console.debug(&format!("Download Complete: {}", success));
 
 			let decoded = decode_path(&filepath.unwrap().to_str().unwrap());
 
 			let new_path = match !download_path.is_empty() {
 				true => match !export_image.is_empty() {
 					true => {
 						let path = PathBuf::from(&export_image);
@@ -109,30 +106,30 @@
 						path.to_path_buf()
 					}
 				},
 
 				false => decoded.to_path_buf(),
 			};
 
-			console.debug(&format!("\nOriginal Path: {:?}", decoded));
+			console.debug(&format!("Original Path: {:?}", decoded));
 			console.debug(&format!("New Path: {:?}", new_path));
 
 			let dir = new_path.parent().unwrap();
 			match !dir.exists() {
 				true => {
-					console.debug(&format!("\nCreating directory: {:?}", dir));
+					console.debug(&format!("Creating directory: {:?}", dir));
 					if let Err(error) = create_dir_all(dir) {
 						console.error(&format!("Error creating directory: {}", error));
 					}
 				}
 				false => {}
 			}
 
 			match copy(&decoded, &new_path) {
-				Err(error) => console.error(&format!("\nError copying file: {}", error)),
+				Err(error) => console.error(&format!("Error copying file: {}", error)),
 				Ok(_) => {
 					if is_export {
 						proxy.send_event(UserEvent::CloseWindow(window_id)).unwrap_or_default();
 					}
 					if let Err(error) = remove_file(&decoded) {
 						console.error(&format!("Error deleting file: {}", error));
 					}
@@ -186,15 +183,15 @@
 					console.error(&format!("Error opening file: {}", error));
 				}
 			}
 		}
 		// WindowEvent::NewWindow
 		#[cfg(not(target_os = "windows"))]
 		Event::UserEvent(UserEvent::NewWindow(uri, window_icon)) => {
-			console.debug(&format!("\nNew Window Requested: {}", uri));
+			console.debug(&format!("New Window Requested: {}", uri));
 			match uri.starts_with("http://") || uri.starts_with("https://") {
 				true => {
 					let pre_window = WindowBuilder::new()
 						.with_title(uri.to_string())
 						.with_window_icon(window_icon)
 						.with_inner_size(LogicalSize::new(1300, 900))
 						.with_resizable(true)
```

### Comparing `pywry-0.5.8/src/handlers.rs` & `pywry-0.5.9/src/handlers.rs`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,17 @@
 				}
 			}
 		})
 		.with_ipc_handler({
 			let proxy = proxy.clone();
 			move |_, string| match string.as_str() {
 				_ if string.starts_with("#PYWRY_RESULT:") => {
-					let result = string.replace("#PYWRY_RESULT:", "").to_string();
-					proxy.send_event(UserEvent::STDout(result)).unwrap_or_default();
+					proxy
+						.send_event(UserEvent::STDout(string[14..].to_string()))
+						.unwrap_or_default();
 
 					if !is_headless {
 						proxy.send_event(UserEvent::CloseWindow(window_id)).unwrap_or_default();
 					}
 				}
 				_ if string.starts_with("data:") => {
 					proxy.send_event(UserEvent::BlobChunk(Some(string))).unwrap_or_default();
```

### Comparing `pywry-0.5.8/src/headless.rs` & `pywry-0.5.9/src/headless.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.8/src/lib.rs` & `pywry-0.5.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.8/src/pipe.rs` & `pywry-0.5.9/src/pipe.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.8/src/structs.rs` & `pywry-0.5.9/src/structs.rs`

 * *Files 8% similar despite different names*

```diff
@@ -100,24 +100,57 @@
 	NewPlot(String, WindowId),
 	OpenFile(Option<PathBuf>),
 	STDout(String),
 	#[cfg(not(target_os = "windows"))]
 	NewWindow(String, Option<Icon>),
 }
 
+pub struct WebViewOptions {
+	/// URL to be loaded when the webview is ready.
+	pub url: String,
+	/// JavaScript code to be injected when the webview is ready.
+	pub init_script: Option<String>,
+}
+
+impl Default for WebViewOptions {
+	/// Returns a default set of WebViewOptions.
+	fn default() -> Self {
+		Self { url: "wry://localhost".to_string(), init_script: None }
+	}
+}
+
+impl WebViewOptions {
+	pub fn new() -> Self {
+		Self::default()
+	}
+
+	/// Sets the URL to be loaded when the webview is ready.
+	pub fn with_url(mut self, url: String) -> Self {
+		self.url = url;
+		self
+	}
+
+	/// Sets the JavaScript code to be injected when the webview is ready.
+	pub fn with_init_script(mut self, init_script: String) -> Self {
+		self.init_script = Some(init_script);
+		self
+	}
+}
+
 pub struct Showable {
 	pub content: String,
 	pub title: String,
 	pub height: Option<u32>,
 	pub width: Option<u32>,
 	pub icon: String,
 	pub data: Option<Value>,
 	pub download_path: String,
 	pub export_image: String,
 	pub theme: Theme,
+	pub options: WebViewOptions,
 }
 
 impl Showable {
 	pub fn new(raw_json: &str) -> Option<Self> {
 		match Self::from_json(raw_json) {
 			Some(item) => Some(item),
 			None => Some(Self::default()),
@@ -145,27 +178,35 @@
 		let icon = json["icon"].as_str().unwrap_or_default().to_string();
 		let title = json["title"].as_str().unwrap_or_default().to_string();
 		let mut height: Option<u32> =
 			json["height"].as_u64().and_then(|x| u32::try_from(x).ok());
 		let mut width: Option<u32> =
 			json["width"].as_u64().and_then(|x| u32::try_from(x).ok());
 		let mut theme = Theme::Light;
+		let mut options = WebViewOptions::new();
 
 		if !json_data.is_null() {
 			theme = match json_data["theme"].as_str().unwrap_or_default() {
 				"dark" => Theme::Dark,
 				"light" => Theme::Light,
 				_ => theme,
 			};
 			if json_data["layout"].is_object() {
 				let raw_width = json_data["layout"]["width"].as_u64().unwrap_or(800);
 				let raw_height = json_data["layout"]["height"].as_u64().unwrap_or(600);
 				width = Some(u32::try_from(raw_width).unwrap_or(800));
 				height = Some(u32::try_from(raw_height).unwrap_or(600));
 			}
+			if json_data["url"].is_string() {
+				options = options.with_url(json_data["url"].as_str().unwrap().to_string());
+			}
+			if json_data["init_script"].is_string() {
+				options = options
+					.with_init_script(json_data["init_script"].as_str().unwrap().to_string());
+			}
 		}
 
 		let export_image = json["export_image"].as_str().unwrap_or_default().to_string();
 		let download_path = json["download_path"].as_str().unwrap_or_default().to_string();
 
 		Some(Self {
 			content,
@@ -173,14 +214,15 @@
 			height,
 			width,
 			icon,
 			data: Some(json_data),
 			download_path,
 			export_image,
 			theme,
+			options,
 		})
 	}
 }
 
 impl Default for Showable {
 	fn default() -> Self {
 		Self {
@@ -193,14 +235,15 @@
 			height: None,
 			width: None,
 			icon: "".to_string(),
 			data: None,
 			download_path: "".to_string(),
 			export_image: "".to_string(),
 			theme: Theme::Light,
+			options: WebViewOptions::default(),
 		}
 	}
 }
 
 pub struct ShowableHeadless {
 	pub data: Option<Value>,
 	pub export_image: String,
```

### Comparing `pywry-0.5.8/src/utils.rs` & `pywry-0.5.9/src/utils.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.8/src/window.rs` & `pywry-0.5.9/src/window.rs`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	collections::HashMap,
 	fs::{canonicalize, read},
 	sync::mpsc::{Receiver, Sender},
 };
 
 use wry::{
 	application::{
-		dpi::LogicalSize,
+		dpi::{LogicalSize, PhysicalPosition},
 		event_loop::{ControlFlow, EventLoop, EventLoopProxy, EventLoopWindowTarget},
 		window::{Theme, WindowBuilder, WindowId},
 	},
 	http::{header::CONTENT_TYPE, Response},
 	webview::{WebView, WebViewBuilder},
 };
 
@@ -43,16 +43,26 @@
 			let mut dev_tools_html = DEV_TOOLS_HTML.as_bytes().to_vec();
 			dev_tools_html.extend(content);
 			dev_tools_html
 		}
 		false => content,
 	};
 
+	let json_data = to_show.data.clone().unwrap_or_default();
+	console.debug(&format!("json_data: {}", json_data));
+
+	let screen_size = event_loop.available_monitors().nth(0).unwrap().size();
+	let window_size = (to_show.width.unwrap_or(800), to_show.height.unwrap_or(600));
+
 	let mut pre_window = WindowBuilder::new()
 		.with_title(to_show.title)
+		.with_position(PhysicalPosition::new(
+			(screen_size.width / 2) - (window_size.0 / 2) + (rand::random::<u32>() % 100),
+			(screen_size.height / 2) - (window_size.1 / 2) + (rand::random::<u32>() % 100),
+		))
 		.with_window_icon(get_icon(&window_icon))
 		.with_min_inner_size(LogicalSize::new(800, 450))
 		.with_theme(Some(Theme::Dark));
 
 	if to_show.height.is_some() && to_show.width.is_some() {
 		pre_window = pre_window.with_inner_size(LogicalSize::new(
 			to_show.width.unwrap_or(800) + 80,
@@ -61,15 +71,15 @@
 	}
 
 	let window = match pre_window.build(event_loop) {
 		Err(error) => return Err(error.to_string()),
 		Ok(item) => item,
 	};
 
-	let minimized = !to_show.export_image.is_empty();
+	let minimized = !to_show.export_image.is_empty() && !console.active;
 	if minimized {
 		window.set_visible(false);
 		window.set_maximized(false);
 	} else {
 		window.set_always_on_top(true);
 	}
 
@@ -80,18 +90,19 @@
 		_ => (255, 255, 255, 255),
 	};
 
 	let webview = match WebViewBuilder::new(window) {
 		Err(error2) => return Err(error2.to_string()),
 		Ok(item) => item,
 	};
-	let protocol = webview
-		.with_background_color(background_color)
-		.with_hotkeys_zoom(true)
-		.with_custom_protocol("wry".into(), move |request| {
+	let protocol =
+		webview.with_background_color(background_color).with_hotkeys_zoom(true);
+
+	let protocol = match to_show.options.url.starts_with("wry://") {
+		true => protocol.with_custom_protocol("wry".into(), move |request| {
 			let path = request.uri().path();
 			let clean_path = &path[1..];
 			let content = content.clone();
 			let mut mime = mime_guess::from_path("index.html");
 
 			let content = if path == "/" {
 				content.into()
@@ -110,15 +121,18 @@
 				.unwrap_or_else(|| "text/plain".to_string());
 
 			Response::builder()
 				.header(CONTENT_TYPE, mimetype)
 				.header("Access-Control-Allow-Origin", "null")
 				.body(content)
 				.map_err(Into::into)
-		});
+		}),
+		false => protocol,
+	};
+
 	let export_image = to_show.export_image.clone();
 	let _is_export = !export_image.is_empty();
 	let download_path = to_show.download_path.clone();
 
 	let init_view = match !to_show.data.is_none() {
 		true => {
 			let variable_value =
@@ -145,15 +159,20 @@
 		window_id,
 		download_path,
 		export_image,
 		&window_icon,
 		Some(false),
 	);
 
-	return match init_view.with_devtools(console.active).with_url("wry://localhost") {
+	let init_view = match to_show.options.init_script.is_some() {
+		true => init_view.with_initialization_script(&to_show.options.init_script.unwrap()),
+		false => init_view,
+	};
+
+	return match init_view.with_devtools(console.active).with_url(&to_show.options.url) {
 		Err(error3) => return Err(error3.to_string()),
 		Ok(subitem) => match subitem.build() {
 			Err(error4) => return Err(error4.to_string()),
 			Ok(sub2item) => {
 				if !minimized {
 					let proxy = proxy.clone();
 					proxy.send_event(UserEvent::NewWindowCreated(window_id)).unwrap_or_default();
@@ -189,15 +208,15 @@
 
 	event_loop.run(move |event, event_loop, control_flow| {
 		*control_flow = ControlFlow::Poll;
 
 		let response = receiver.try_recv().unwrap_or_default();
 
 		if !response.is_empty() {
-			console.debug("\nReceived response");
+			console.debug("Received message from Python");
 
 			let chart = Showable::new(&response).unwrap_or_default();
 			match create_new_window(chart, &event_loop, &proxy, console) {
 				Err(error) => console.error(&format!("Error creating window: {}", error)),
 				Ok(new_window) => {
 					webviews.insert(new_window.0, new_window.1);
 				}
```

### Comparing `pywry-0.5.8/PKG-INFO` & `pywry-0.5.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywry
-Version: 0.5.8
+Version: 0.5.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Requires-Dist: setproctitle
@@ -171,7 +171,11 @@
 
 ### Troubleshooting Linux
 
 #### `"/lib/x86_64-linux-gnu/libgio-2.0.so.0: undefined symbol: g_module_open_full"`
 
 This is a known issue with the `gio` library. You can fix it by installing the `libglib2.0-dev` package.
 
+
+
+PyWry is a project that aims to provide Python bindings for WRY, a cross-platform webview library. WRY is a trademark of the Tauri Program within the Commons Conservancy and PyWry is not officially endorsed or supported by them. PyWry is an independent and community-driven effort that respects the original goals and values of Tauri and WRY. PyWry does not claim any ownership or affiliation with WRY or the Tauri Program.
+
```

