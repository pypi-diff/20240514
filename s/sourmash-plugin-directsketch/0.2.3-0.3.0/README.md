# Comparing `tmp/sourmash_plugin_directsketch-0.2.3.tar.gz` & `tmp/sourmash_plugin_directsketch-0.3.0.tar.gz`

## Comparing `sourmash_plugin_directsketch-0.2.3.tar` & `sourmash_plugin_directsketch-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,27 @@
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.2.3/Cargo.toml
--rw-r--r--   0      501       20      405 2024-05-09 18:23:51.000000 sourmash_plugin_directsketch-0.2.3/.github/dependabot.yml
--rw-r--r--   0      501       20     1421 2024-05-09 18:23:54.000000 sourmash_plugin_directsketch-0.2.3/.github/workflows/build-test.yml
--rw-r--r--   0      501       20      718 2024-04-26 03:30:23.000000 sourmash_plugin_directsketch-0.2.3/.gitignore
--rw-r--r--   0      501       20     1540 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.3/LICENSE
--rw-r--r--   0      501       20      368 2024-05-01 15:59:57.000000 sourmash_plugin_directsketch-0.2.3/Makefile
--rw-r--r--   0      501       20     3377 2024-05-09 18:23:51.000000 sourmash_plugin_directsketch-0.2.3/README.md
--rw-r--r--   0      501       20      176 2024-04-30 23:49:37.000000 sourmash_plugin_directsketch-0.2.3/environment.yml
--rw-r--r--   0      501       20    25831 2024-05-10 03:35:26.000000 sourmash_plugin_directsketch-0.2.3/src/directsketch.rs
--rw-r--r--   0      501       20     2359 2024-05-09 18:23:51.000000 sourmash_plugin_directsketch-0.2.3/src/lib.rs
--rw-r--r--   0      501       20     4597 2024-05-09 18:23:51.000000 sourmash_plugin_directsketch-0.2.3/src/python/sourmash_plugin_directsketch/__init__.py
--rw-r--r--   0      501       20     5730 2024-05-07 17:31:28.000000 sourmash_plugin_directsketch-0.2.3/src/utils.rs
--rw-r--r--   0      501       20      410 2024-05-09 18:23:51.000000 sourmash_plugin_directsketch-0.2.3/tests/conftest.py
--rw-r--r--   0      501       20     6849 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.3/tests/sourmash_tst_utils.py
--rw-r--r--   0      501       20        0 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/.notempty
--rw-r--r--   0      501       20    44471 2024-04-26 18:22:33.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/GCA_000175555.1.sig.gz
--rw-r--r--   0      501       20    20407 2024-04-27 01:42:18.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/GCA_000961135.2.protein.sig.gz
--rw-r--r--   0      501       20    29259 2024-04-26 18:04:28.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/GCA_000961135.2.sig.gz
--rw-r--r--   0      501       20      497 2024-04-27 02:01:15.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/acc.csv
--rw-r--r--   0      501       20   798402 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/out_fastas/GCA_000175555.1_genomic.fna.gz
--rw-r--r--   0      501       20   526013 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/out_fastas/GCA_000961135.2_genomic.fna.gz
--rw-r--r--   0      501       20   314606 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/out_fastas/GCA_000961135.2_protein.faa.gz
--rw-r--r--   0      501       20   798402 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/outputs/GCA_000175555.1_genomic.fna.gz
--rw-r--r--   0      501       20     7793 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/outputs/GCA_000337115.1_assembly_report.txt
--rw-r--r--   0      501       20  1118769 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/outputs/GCA_000337115.1_genomic.fna.gz
--rw-r--r--   0      501       20     1201 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/outputs/GCA_000337115.1_md5checksums.txt
--rw-r--r--   0      501       20   702342 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/outputs/GCA_000337115.1_protein.faa.gz
--rw-r--r--   0      501       20    36700 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/outputs/GCA_000961135.2_assembly_report.txt
--rw-r--r--   0      501       20   526013 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/outputs/GCA_000961135.2_genomic.fna.gz
--rw-r--r--   0      501       20     1201 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/outputs/GCA_000961135.2_md5checksums.txt
--rw-r--r--   0      501       20   314606 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/outputs/GCA_000961135.2_protein.faa.gz
--rw-r--r--   0      501       20   735547 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/outputs/GCA_001950595.1_genomic.fna.gz
--rw-r--r--   0      501       20   118778 2024-04-27 00:46:05.000000 sourmash_plugin_directsketch-0.2.3/tests/test-data/test.zip
--rw-r--r--   0      501       20    11422 2024-05-09 18:23:51.000000 sourmash_plugin_directsketch-0.2.3/tests/test_gbsketch.py
--rw-r--r--   0      501       20    63405 2024-05-10 03:35:58.000000 sourmash_plugin_directsketch-0.2.3/Cargo.lock
--rw-r--r--   0      501       20      966 2024-05-09 18:23:54.000000 sourmash_plugin_directsketch-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4047 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.3.0/Cargo.toml
+-rw-r--r--   0      501       20      405 2024-05-09 18:23:51.000000 sourmash_plugin_directsketch-0.3.0/.github/dependabot.yml
+-rw-r--r--   0      501       20     1421 2024-05-09 18:23:54.000000 sourmash_plugin_directsketch-0.3.0/.github/workflows/build-test.yml
+-rw-r--r--   0      501       20      718 2024-04-26 03:30:23.000000 sourmash_plugin_directsketch-0.3.0/.gitignore
+-rw-r--r--   0      501       20     1540 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.3.0/LICENSE
+-rw-r--r--   0      501       20      368 2024-05-01 15:59:57.000000 sourmash_plugin_directsketch-0.3.0/Makefile
+-rw-r--r--   0      501       20     4103 2024-05-13 23:02:21.000000 sourmash_plugin_directsketch-0.3.0/README.md
+-rw-r--r--   0      501       20      176 2024-04-30 23:49:37.000000 sourmash_plugin_directsketch-0.3.0/environment.yml
+-rw-r--r--   0      501       20    26384 2024-05-13 23:02:21.000000 sourmash_plugin_directsketch-0.3.0/src/directsketch.rs
+-rw-r--r--   0      501       20     2367 2024-05-13 23:02:21.000000 sourmash_plugin_directsketch-0.3.0/src/lib.rs
+-rw-r--r--   0      501       20     4892 2024-05-13 23:02:21.000000 sourmash_plugin_directsketch-0.3.0/src/python/sourmash_plugin_directsketch/__init__.py
+-rw-r--r--   0      501       20    11467 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/src/utils.rs
+-rw-r--r--   0      501       20      410 2024-05-09 18:23:51.000000 sourmash_plugin_directsketch-0.3.0/tests/conftest.py
+-rw-r--r--   0      501       20     6849 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.3.0/tests/sourmash_tst_utils.py
+-rw-r--r--   0      501       20        0 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/.notempty
+-rw-r--r--   0      501       20    18550 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/GCA_000175535.1.sig.gz
+-rw-r--r--   0      501       20    35505 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/GCA_000193795.2.sig.gz
+-rw-r--r--   0      501       20    23022 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/GCA_000961135.2.protein.sig.gz
+-rw-r--r--   0      501       20    30635 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/GCA_000961135.2.sig.gz
+-rw-r--r--   0      501       20      221 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/acc-cols.csv
+-rw-r--r--   0      501       20      115 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/acc-version.csv
+-rw-r--r--   0      501       20      386 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/acc-with-ftppath.csv
+-rw-r--r--   0      501       20      219 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/acc.csv
+-rw-r--r--   0      501       20    17370 2024-05-13 23:02:21.000000 sourmash_plugin_directsketch-0.3.0/tests/test_gbsketch.py
+-rw-r--r--   0      501       20    63405 2024-05-13 23:04:06.000000 sourmash_plugin_directsketch-0.3.0/Cargo.lock
+-rw-r--r--   0      501       20      966 2024-05-09 18:23:54.000000 sourmash_plugin_directsketch-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4773 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.3.0/PKG-INFO
```

### Comparing `sourmash_plugin_directsketch-0.2.3/Cargo.toml` & `sourmash_plugin_directsketch-0.3.0/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [package]
 name = "sourmash_plugin_directsketch"
-version = "0.2.3"
+version = "0.3.0"
 edition = "2021"
 
 [lib]
 name = "sourmash_plugin_directsketch"
 crate-type = ["cdylib"]
 
 [dependencies]
```

### Comparing `sourmash_plugin_directsketch-0.2.3/.github/workflows/build-test.yml` & `sourmash_plugin_directsketch-0.3.0/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.3/.gitignore` & `sourmash_plugin_directsketch-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.3/LICENSE` & `sourmash_plugin_directsketch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.3/README.md` & `sourmash_plugin_directsketch-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -12,23 +12,37 @@
 ## Installation
 
 ```
 pip install sourmash_plugin_directsketch
 ```
 
 ## Usage
+
+### Create an input file
+
 First, create a file, e.g. `acc.csv` with GenBank identifiers and sketch names.
 ```
-ident,name
-GCA_000961135.2,GCA_000961135.2 Candidatus Aramenus sulfurataquae isolate AZ1-45
-GCA_000175555.1,GCA_000175555.1 ACUK01000506.1 Saccharolobus solfataricus 98/2
+accession,name,ftp_path
+GCA_000961135.2,GCA_000961135.2 Candidatus Aramenus sulfurataquae isolate AZ1-45,
+GCA_000175555.1,GCA_000175555.1 ACUK01000506.1 Saccharolobus solfataricus 98/2,
 ```
-> Extra columns are ok, as long as the first two columns contain the identifier and sketch name
+> Three columns must be present: `accession`, `name`, and `ftp_path`. The `ftp_path` column can be empty, but no additional columns may be present.
+
+#### What is ftp_path?
+
+If you do not provide an `ftp_path`, `gbsketch` will use the accession to find the `ftp_path` for you.
+
+If you choose to provide it, `ftp_path` must be the `ftp_path` column from NCBI's assembly summary files.
+
+For reference:
+
+- example `ftp_path`: [https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/036/600/915/GCA_036600915.1_ASM3660091v1](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/036/600/915/GCA_036600915.1_ASM3660091v1)
+- bacteria assembly summary file: [https://ftp.ncbi.nih.gov/genomes/genbank/bacteria/assembly_summary.txt](https://ftp.ncbi.nih.gov/genomes/genbank/bacteria/assembly_summary.txt)
 
-Run:
+### Run:
 
 To run the test accession file at `tests/test-data/acc.csv`, run:
 ```
 sourmash scripts gbsketch tests/test-data/acc.csv -o test.zip -f out_fastas -k --failed test.failed.csv -p dna,k=21,k=31,scaled=1000,abund -p protein,k=10,scaled=100,abund -r 1
 ```
 
 Full Usage:
```

### Comparing `sourmash_plugin_directsketch-0.2.3/src/directsketch.rs` & `sourmash_plugin_directsketch-0.3.0/src/directsketch.rs`

 * *Files 5% similar despite different names*

```diff
@@ -18,134 +18,102 @@
 use tokio_util::compat::Compat;
 
 use pyo3::prelude::*;
 
 use sourmash::manifest::{Manifest, Record};
 use sourmash::signature::Signature;
 
-use crate::utils::{build_siginfo, load_accession_info, parse_params_str};
+use crate::utils::{
+    build_siginfo, load_gbassembly_info, parse_params_str, GBAssemblyData, GenBankFileType,
+};
+use reqwest::Url;
 
-#[allow(dead_code)]
-enum GenBankFileType {
-    Genomic,
-    Protein,
-    AssemblyReport,
-    Checksum,
-}
-
-impl GenBankFileType {
-    fn suffix(&self) -> &'static str {
-        match self {
-            GenBankFileType::Genomic => "_genomic.fna.gz",
-            GenBankFileType::Protein => "_protein.faa.gz",
-            GenBankFileType::AssemblyReport => "_assembly_report.txt",
-            GenBankFileType::Checksum => "md5checksums.txt",
-        }
-    }
+async fn find_genome_directory(
+    client: &Client,
+    db: &str,
+    number_path: &str,
+    accession: &str,
+    acc_number: &str,
+    version: &str,
+) -> Result<(Url, String)> {
+    let base_url = format!(
+        "https://ftp.ncbi.nlm.nih.gov/genomes/all/{}/{}",
+        db, number_path
+    );
+    let directory_response = client.get(&base_url).send().await?;
 
-    //use for checksums
-    fn server_filename(&self, full_name: &str) -> String {
-        format!("{}{}", full_name, self.suffix())
+    if !directory_response.status().is_success() {
+        return Err(anyhow!(
+            "Failed to open genome directory: HTTP {}, {}",
+            directory_response.status(),
+            directory_response
+                .status()
+                .canonical_reason()
+                .unwrap_or("Unknown reason")
+        ));
     }
+    let text = directory_response.text().await?;
+    let link_regex = Regex::new(r#"<a href="([^"]+)/""#)?;
 
-    fn filename_to_write(&self, accession: &str) -> String {
-        match self {
-            GenBankFileType::Checksum => format!("{}_{}", accession, self.suffix()),
-            _ => format!("{}{}", accession, self.suffix()),
-        }
-    }
+    for cap in link_regex.captures_iter(&text) {
+        let name = &cap[1];
 
-    fn url(&self, base_url: &str, full_name: &str) -> String {
-        match self {
-            GenBankFileType::Checksum => format!("{}/{}", base_url, self.suffix()),
-            _ => format!("{}/{}{}", base_url, full_name, self.suffix()),
-        }
-    }
+        // Use acc numerical identifier and version as expected pattern
+        let expected_pattern = format!("{}.{}", acc_number, version);
 
-    fn moltype(&self) -> String {
-        match self {
-            GenBankFileType::Genomic => "DNA".to_string(),
-            GenBankFileType::Protein => "protein".to_string(),
-            _ => "".to_string(),
+        // Check if directory name contains contains the right acc number and version
+        if name.contains(&expected_pattern) {
+            let url = format!("{}/{}", base_url, name).parse()?;
+            return Ok((url, name.to_string()));
         }
     }
+    Err(anyhow!(
+        "No matching directory found for accession {}",
+        accession
+    ))
 }
 
-async fn fetch_genbank_filename(client: &Client, accession: &str) -> Result<(String, String)> {
+async fn fetch_genbank_filename(
+    client: &Client,
+    accession: &str,
+    url: Option<Url>,
+) -> Result<(Url, String)> {
     let (db, acc) = accession
         .trim()
         .split_once('_')
         .ok_or_else(|| anyhow!("Invalid accession format"))?;
-    let (number, _) = acc.split_once('.').unwrap_or((acc, "1"));
-    let number_path = number
+    let (acc_number, version) = acc.split_once('.').unwrap_or((acc, "1"));
+    let number_path = acc_number
         .chars()
         .collect::<Vec<_>>()
         .chunks(3)
         .map(|chunk| chunk.iter().collect::<String>())
         .collect::<Vec<_>>()
         .join("/");
 
-    let base_url = format!(
-        "https://ftp.ncbi.nlm.nih.gov/genomes/all/{}/{}",
-        db, number_path
-    );
-    let directory_response = client.get(&base_url).send().await;
-
-    match directory_response {
-        Ok(response) => {
-            if !response.status().is_success() {
-                return Err(anyhow!(
-                    "Failed to open genome directory: HTTP {}, {}",
-                    response.status(),
-                    response
-                        .status()
-                        .canonical_reason()
-                        .unwrap_or("Unknown reason")
-                ));
-            }
-
-            let text = response.text().await?;
-            let link_regex = Regex::new(r#"<a href="([^"]*)""#)?;
-
-            for cap in link_regex.captures_iter(&text) {
-                let name = &cap[1];
-                let clean_name = if name.ends_with('/') {
-                    name.strip_suffix('/').unwrap()
-                } else {
-                    name
-                };
+    let (url, name) = if let Some(url) = url {
+        let url_parts: Vec<&str> = url
+            .path_segments()
+            .ok_or_else(|| anyhow!("Failed to extract path segments from URL"))?
+            .collect();
+        let name = url_parts
+            .last()
+            .ok_or_else(|| anyhow!("Failed to extract name from URL"))?
+            .to_string();
+        (url, name)
+    } else {
+        find_genome_directory(client, db, &number_path, accession, acc_number, version).await?
+    };
 
-                if clean_name.starts_with(db)
-                    && clean_name
-                        .split('_')
-                        .nth(1)
-                        .map_or(false, |x| x.starts_with(number))
-                {
-                    return Ok((format!("{}/{}", base_url, clean_name), clean_name.into()));
-                }
-            }
-            Err(anyhow!(
-                "No matching directory found for accession {}",
-                accession
-            ))
-        }
-        Err(e) => {
-            // eprintln!("HTTP request failed for accession {}: {}", accession, e);
-            Err(anyhow!(
-                "HTTP request failed for accession {}: {}",
-                accession,
-                e
-            ))
-        }
-    }
+    Ok((url, name))
 }
 
-async fn download_and_parse_md5(client: &Client, url: &str) -> Result<HashMap<String, String>> {
+async fn download_and_parse_md5(client: &Client, url: &Url) -> Result<HashMap<String, String>> {
     let response = client
-        .get(url)
+        .get(url.clone())
         .send()
         .await
         .context("Failed to send request")?;
 
     let content = response
         .text()
         .await
@@ -171,23 +139,23 @@
 
     Ok(checksums)
 }
 
 // download and return data directly instead of saving to file
 async fn download_with_retry(
     client: &Client,
-    url: &str,
+    url: &Url,
     expected_md5: Option<&str>,
     retry_count: u32,
 ) -> Result<Vec<u8>> {
     let mut attempts = retry_count;
     let mut last_error: Option<anyhow::Error> = None;
 
     while attempts > 0 {
-        let response = client.get(url).send().await;
+        let response = client.get(url.clone()).send().await;
 
         match response {
             Ok(resp) if resp.status().is_success() => {
                 let data = resp
                     .bytes()
                     .await
                     .context("Failed to read bytes from response")?;
@@ -266,68 +234,69 @@
                 set_name = true;
             }
         }
         Result::<Vec<Signature>, anyhow::Error>::Ok(sigs)
     })
     .await?
 }
-
 pub struct FailedDownload {
     accession: String,
     name: String,
-    url: String,
+    url: Option<Url>,
     moltype: String,
 }
 
 #[allow(clippy::too_many_arguments)]
 async fn dl_sketch_accession(
     client: &Client,
-    accession: String,
-    name: String,
+    accinfo: GBAssemblyData,
     location: &PathBuf,
     retry: Option<u32>,
     keep_fastas: bool,
     dna_sigs: Vec<Signature>,
     prot_sigs: Vec<Signature>,
     genomes_only: bool,
     proteomes_only: bool,
     download_only: bool,
 ) -> Result<(Vec<Signature>, Vec<FailedDownload>)> {
     let retry_count = retry.unwrap_or(3); // Default retry count
     let mut sigs = Vec::<Signature>::new();
     let mut failed = Vec::<FailedDownload>::new();
 
-    // keep track of any accessions for which we fail to find URLs
-    let (base_url, full_name) = match fetch_genbank_filename(client, accession.as_str()).await {
-        Ok(result) => result,
-        Err(_err) => {
-            // Add accession to failed downloads with each moltype
-            if !proteomes_only {
-                let failed_download_dna = FailedDownload {
-                    accession: accession.clone(),
-                    name: name.clone(),
-                    url: "".to_string(),
-                    moltype: "dna".to_string(),
-                };
-                failed.push(failed_download_dna);
-            }
-            if !genomes_only {
-                let failed_download_protein = FailedDownload {
-                    accession: accession.clone(),
-                    name: name.clone(),
-                    url: "".to_string(),
-                    moltype: "protein".to_string(),
-                };
-                failed.push(failed_download_protein);
-            }
+    let name = accinfo.name;
+    let accession = accinfo.accession;
 
-            return Ok((sigs, failed));
-        }
-    };
+    // keep track of any accessions for which we fail to find URLs
+    let (base_url, full_name) =
+        match fetch_genbank_filename(client, accession.as_str(), accinfo.url).await {
+            Ok(result) => result,
+            Err(_err) => {
+                // Add accession to failed downloads with each moltype
+                if !proteomes_only {
+                    let failed_download_dna = FailedDownload {
+                        accession: accession.clone(),
+                        name: name.clone(),
+                        url: None,
+                        moltype: "dna".to_string(),
+                    };
+                    failed.push(failed_download_dna);
+                }
+                if !genomes_only {
+                    let failed_download_protein = FailedDownload {
+                        accession: accession.clone(),
+                        name: name.clone(),
+                        url: None,
+                        moltype: "protein".to_string(),
+                    };
+                    failed.push(failed_download_protein);
+                }
 
+                return Ok((sigs, failed));
+            }
+        };
     let md5sum_url = GenBankFileType::Checksum.url(&base_url, &full_name);
 
     let checksums = match download_and_parse_md5(client, &md5sum_url).await {
         Ok(cs) => cs,
         Err(e) => {
             return Err(e);
         }
@@ -343,26 +312,25 @@
     } else if proteomes_only {
         file_types = vec![GenBankFileType::Protein];
     }
 
     for file_type in &file_types {
         let url = file_type.url(&base_url, &full_name);
         let expected_md5 = checksums.get(&file_type.server_filename(&full_name));
-        // let checksum = checksums
         let data =
             match download_with_retry(client, &url, expected_md5.map(|x| x.as_str()), retry_count)
                 .await
             {
                 Ok(data) => data,
                 Err(_err) => {
                     // here --> keep track of accession errors + filetype
                     let failed_download = FailedDownload {
                         accession: accession.clone(),
                         name: name.clone(),
-                        url: url.clone(),
+                        url: Some(url),
                         moltype: file_type.moltype(),
                     };
                     failed.push(failed_download);
                     continue;
                 }
             };
         let file_name = file_type.filename_to_write(&accession);
@@ -450,90 +418,92 @@
         .write_entry_whole(builder, &gzipped_buffer)
         .await
         .map_err(|e| anyhow!("Error writing zip entry: {}", e))
 }
 
 pub fn sigwriter_handle(
     mut recv_sigs: tokio::sync::mpsc::Receiver<Vec<Signature>>,
-    output_sigs: String,
+    output_sigs: Option<String>,
     error_sender: tokio::sync::mpsc::Sender<anyhow::Error>,
 ) -> tokio::task::JoinHandle<()> {
     tokio::spawn(async move {
         let mut md5sum_occurrences = HashMap::new();
         let mut manifest_rows = Vec::new();
         let mut wrote_sigs = false;
-        let outpath: PathBuf = output_sigs.into();
+        if let Some(outpath) = output_sigs {
+            let outpath: PathBuf = outpath.into();
 
-        let file = match File::create(&outpath).await {
-            Ok(file) => file,
-            Err(e) => {
-                let error =
-                    anyhow::Error::new(e).context("Failed to create file at specified path");
-                let _ = error_sender.send(error).await; // Send the error through the channel
-                return; // Simply exit the task as error handling is managed elsewhere
-            }
-        };
-        let mut zip_writer = ZipFileWriter::with_tokio(file);
+            let file = match File::create(&outpath).await {
+                Ok(file) => file,
+                Err(e) => {
+                    let error =
+                        anyhow::Error::new(e).context("Failed to create file at specified path");
+                    let _ = error_sender.send(error).await; // Send the error through the channel
+                    return; // Simply exit the task as error handling is managed elsewhere
+                }
+            };
+            let mut zip_writer = ZipFileWriter::with_tokio(file);
 
-        while let Some(sigs) = recv_sigs.recv().await {
-            for sig in sigs {
-                match write_sig(
-                    &sig,
-                    &mut md5sum_occurrences,
-                    &mut manifest_rows,
-                    &mut zip_writer,
-                )
-                .await
-                {
-                    Ok(_) => wrote_sigs = true,
-                    Err(e) => {
-                        let error = e.context("Error processing signature");
-                        if (error_sender.send(error).await).is_err() {
-                            return; // Exit on failure to send error
+            while let Some(sigs) = recv_sigs.recv().await {
+                for sig in sigs {
+                    match write_sig(
+                        &sig,
+                        &mut md5sum_occurrences,
+                        &mut manifest_rows,
+                        &mut zip_writer,
+                    )
+                    .await
+                    {
+                        Ok(_) => wrote_sigs = true,
+                        Err(e) => {
+                            let error = e.context("Error processing signature");
+                            if (error_sender.send(error).await).is_err() {
+                                return; // Exit on failure to send error
+                            }
                         }
                     }
                 }
             }
-        }
 
-        if wrote_sigs {
-            println!("Writing manifest");
-            let manifest_filename = "SOURMASH-MANIFEST.csv".to_string();
-            let manifest: Manifest = manifest_rows.clone().into();
-            let mut manifest_buffer = Vec::new();
-            manifest
-                .to_writer(&mut manifest_buffer)
-                .expect("Failed to serialize manifest"); // Handle this more gracefully in production
-
-            let now = Utc::now();
-            let builder = ZipEntryBuilder::new(manifest_filename.into(), Compression::Stored)
-                .last_modification_date(ZipDateTime::from_chrono(&now));
+            if wrote_sigs {
+                println!("Writing manifest");
+                let manifest_filename = "SOURMASH-MANIFEST.csv".to_string();
+                let manifest: Manifest = manifest_rows.clone().into();
+                let mut manifest_buffer = Vec::new();
+                manifest
+                    .to_writer(&mut manifest_buffer)
+                    .expect("Failed to serialize manifest"); // Handle this more gracefully in production
+
+                let now = Utc::now();
+                let builder = ZipEntryBuilder::new(manifest_filename.into(), Compression::Stored)
+                    .last_modification_date(ZipDateTime::from_chrono(&now));
 
-            if let Err(e) = zip_writer
-                .write_entry_whole(builder, &manifest_buffer)
-                .await
-            {
-                let error = anyhow::Error::new(e).context("Failed to write manifest to ZIP");
-                let _ = error_sender.send(error).await;
-                return;
-            }
+                if let Err(e) = zip_writer
+                    .write_entry_whole(builder, &manifest_buffer)
+                    .await
+                {
+                    let error = anyhow::Error::new(e).context("Failed to write manifest to ZIP");
+                    let _ = error_sender.send(error).await;
+                    return;
+                }
 
-            if let Err(e) = zip_writer.close().await {
-                let error = anyhow::Error::new(e).context("Failed to close ZIP file");
-                let _ = error_sender.send(error).await;
-                return;
+                if let Err(e) = zip_writer.close().await {
+                    let error = anyhow::Error::new(e).context("Failed to close ZIP file");
+                    let _ = error_sender.send(error).await;
+                    return;
+                }
+            } else {
+                let error = anyhow::Error::new(std::io::Error::new(
+                    std::io::ErrorKind::Other,
+                    "No signatures written",
+                ));
+                let _ = error_sender.send(error).await; // Send error about no signatures written
             }
-        } else {
-            let error = anyhow::Error::new(std::io::Error::new(
-                std::io::ErrorKind::Other,
-                "No signatures written",
-            ));
-            let _ = error_sender.send(error).await; // Send error about no signatures written
         }
-        drop(error_sender);
+        drop(error_sender); // should be dropped automatically as it goes out of scope, but just in case
     })
 }
 
 pub fn failures_handle(
     failed_csv: String,
     mut recv_failed: tokio::sync::mpsc::Receiver<FailedDownload>,
     error_sender: tokio::sync::mpsc::Sender<Error>, // Additional parameter for error channel
@@ -553,16 +523,15 @@
                 while let Some(FailedDownload {
                     accession,
                     name,
                     moltype,
                     url,
                 }) = recv_failed.recv().await
                 {
-                    let record = format!("{},{},{},{}\n", accession, name, moltype, url);
-
+                    let record = format!("{},{},{},{:?}\n", accession, name, moltype, url);
                     // Attempt to write each record
                     if let Err(e) = writer.write_all(record.as_bytes()).await {
                         let error = Error::new(e).context("Failed to write record");
                         let _ = error_sender.send(error).await;
                         continue; // Optionally continue to try to write next records
                     }
                 }
@@ -598,74 +567,103 @@
 }
 
 #[tokio::main]
 #[allow(clippy::too_many_arguments)]
 pub async fn download_and_sketch(
     py: Python,
     input_csv: String,
-    output_sigs: String,
     param_str: String,
     failed_csv: String,
     retry_times: u32,
     fasta_location: String,
     keep_fastas: bool,
     genomes_only: bool,
     proteomes_only: bool,
     download_only: bool,
+    output_sigs: Option<String>,
 ) -> Result<(), anyhow::Error> {
-    // if sig output doesn't end in zip, bail
-    if Path::new(&output_sigs)
-        .extension()
-        .map_or(true, |ext| ext != "zip")
-    {
-        bail!("Output must be a zip file.");
+    // if sig output provided but doesn't end in zip, bail
+    if let Some(ref output_sigs) = output_sigs {
+        if Path::new(&output_sigs)
+            .extension()
+            .map_or(true, |ext| ext != "zip")
+        {
+            bail!("Output must be a zip file.");
+        }
     }
     // set up fasta download path
     let download_path = PathBuf::from(fasta_location);
     if !download_path.exists() {
         create_dir_all(&download_path)?;
     }
 
     // create channels. buffer size here is 4 b/c we can do 3 downloads simultaneously
     let (send_sigs, recv_sigs) = tokio::sync::mpsc::channel::<Vec<Signature>>(4);
     let (send_failed, recv_failed) = tokio::sync::mpsc::channel::<FailedDownload>(4);
-    // // Error channel for handling task errors
+    // Error channel for handling task errors
     let (error_sender, error_receiver) = tokio::sync::mpsc::channel::<anyhow::Error>(1);
 
-    // //  // Set up collector/writing tasks
+    // Set up collector/writing tasks
     let mut handles = Vec::new();
     let sig_handle = sigwriter_handle(recv_sigs, output_sigs, error_sender.clone());
     let failures_handle = failures_handle(failed_csv, recv_failed, error_sender.clone());
     let critical_error_flag = Arc::new(AtomicBool::new(false));
     let error_handle = error_handler(error_receiver, critical_error_flag.clone());
     handles.push(sig_handle);
     handles.push(failures_handle);
     handles.push(error_handle);
 
-    // // Worker tasks
+    // Worker tasks
     let semaphore = Arc::new(Semaphore::new(3)); // Limiting concurrent downloads
     let client = Arc::new(Client::new());
 
     // Open the file containing the accessions synchronously
-    let (accession_info, n_accs) = load_accession_info(input_csv)?;
+    let (accession_info, n_accs) = load_gbassembly_info(input_csv)?;
     if n_accs == 0 {
         bail!("No accessions to download and sketch.")
     }
 
-    // // parse param string into params_vec, print error if fail
+    // parse param string into params_vec, print error if fail
     let param_result = parse_params_str(param_str);
     let params_vec = match param_result {
         Ok(params) => params,
         Err(e) => {
             bail!("Failed to parse params string: {}", e);
         }
     };
     let dna_sig_templates = build_siginfo(&params_vec, "DNA");
     let prot_sig_templates = build_siginfo(&params_vec, "protein");
 
+    let mut genomes_only = genomes_only;
+    let mut proteomes_only = proteomes_only;
+
+    // Check if dna_sig_templates is empty and not keep_fastas
+    if dna_sig_templates.is_empty() && !keep_fastas {
+        eprintln!("No DNA signature templates provided, and --keep-fastas is not set.");
+        proteomes_only = true;
+    }
+    // Check if protein_sig_templates is empty and not keep_fastas
+    if prot_sig_templates.is_empty() && !keep_fastas {
+        eprintln!("No protein signature templates provided, and --keep-fastas is not set.");
+        genomes_only = true;
+    }
+    if genomes_only {
+        if !download_only {
+            eprintln!("Downloading and sketching genomes only.");
+        } else {
+            eprintln!("Downloading genomes only.");
+        }
+    } else if proteomes_only {
+        if !download_only {
+            eprintln!("Downloading and sketching proteomes only.");
+        } else {
+            eprintln!("Downloading proteomes only.");
+        }
+    }
+
     // report every 1 percent (or every 1, whichever is larger)
     let reporting_threshold = std::cmp::max(n_accs / 100, 1);
 
     for (i, accinfo) in accession_info.into_iter().enumerate() {
         py.check_signals()?; // If interrupted, return an Err automatically
         let semaphore_clone = Arc::clone(&semaphore);
         let client_clone = Arc::clone(&client);
@@ -675,44 +673,45 @@
         let send_errors = error_sender.clone();
 
         let dna_sigs = dna_sig_templates.clone();
         let prot_sigs = prot_sig_templates.clone();
 
         tokio::spawn(async move {
             let _permit = semaphore_clone.acquire().await;
-            // Report when the permit is available and processing begins
+            // progress report when the permit is available and processing begins
             if (i + 1) % reporting_threshold == 0 {
                 let percent_processed = (((i + 1) as f64 / n_accs as f64) * 100.0).round();
                 println!(
                     "Starting accession {}/{} ({}%)",
                     (i + 1),
                     n_accs,
                     percent_processed
                 );
             }
             // Perform download and sketch
             let result = dl_sketch_accession(
                 &client_clone,
-                accinfo.accession.clone(),
-                accinfo.name.clone(),
+                accinfo.clone(),
                 &download_path_clone,
                 Some(retry_times),
                 keep_fastas,
                 dna_sigs,
                 prot_sigs,
                 genomes_only,
                 proteomes_only,
                 download_only,
             )
             .await;
             match result {
                 Ok((sigs, failed_downloads)) => {
-                    if let Err(e) = send_sigs.send(sigs).await {
-                        eprintln!("Failed to send signatures: {}", e);
-                        let _ = send_errors.send(e.into()).await; // Send the error through the channel
+                    if !sigs.is_empty() {
+                        if let Err(e) = send_sigs.send(sigs).await {
+                            eprintln!("Failed to send signatures: {}", e);
+                            let _ = send_errors.send(e.into()).await; // Send the error through the channel
+                        }
                     }
                     for fail in failed_downloads {
                         if let Err(e) = send_failed.send(fail).await {
                             eprintln!("Failed to send failed download info: {}", e);
                             let _ = send_errors.send(e.into()).await; // Send the error through the channel
                         }
                     }
```

#### html2text {}

```diff
@@ -3,67 +3,59 @@
 ZipEntryBuilder}; use camino::Utf8PathBuf as PathBuf; use chrono::Utc; use
 needletail::parse_fastx_reader; use regex::Regex; use reqwest::Client; use
 std::collections::HashMap; use std::fs::{self, create_dir_all}; use std::io::
 Cursor; use std::path::Path; use std::sync::atomic::{AtomicBool, Ordering}; use
 std::sync::Arc; use tokio::fs::File; use tokio::io::{AsyncWriteExt, BufWriter};
 use tokio::sync::Semaphore; use tokio_util::compat::Compat; use pyo3::prelude::
 *; use sourmash::manifest::{Manifest, Record}; use sourmash::signature::
-Signature; use crate::utils::{build_siginfo, load_accession_info,
-parse_params_str}; #[allow(dead_code)] enum GenBankFileType { Genomic, Protein,
-AssemblyReport, Checksum, } impl GenBankFileType { fn suffix(&self) -> &'static
-str { match self { GenBankFileType::Genomic => "_genomic.fna.gz",
-GenBankFileType::Protein => "_protein.faa.gz", GenBankFileType::AssemblyReport
-=> "_assembly_report.txt", GenBankFileType::Checksum => "md5checksums.txt", } }
-//use for checksums fn server_filename(&self, full_name: &str) -> String
-{ format!("{}{}", full_name, self.suffix()) } fn filename_to_write(&self,
-accession: &str) -> String { match self { GenBankFileType::Checksum => format!
-("{}_{}", accession, self.suffix()), _ => format!("{}{}", accession,
-self.suffix()), } } fn url(&self, base_url: &str, full_name: &str) -> String
-{ match self { GenBankFileType::Checksum => format!("{}/{}", base_url,
-self.suffix()), _ => format!("{}/{}{}", base_url, full_name, self.suffix()), }
-} fn moltype(&self) -> String { match self { GenBankFileType::Genomic =>
-"DNA".to_string(), GenBankFileType::Protein => "protein".to_string(), _ =>
-"".to_string(), } } } async fn fetch_genbank_filename(client: &Client,
-accession: &str) -> Result<(String, String)> { let (db, acc) = accession .trim
-() .split_once('_') .ok_or_else(|| anyhow!("Invalid accession format"))?; let
-(number, _) = acc.split_once('.').unwrap_or((acc, "1")); let number_path =
-number .chars() .collect::
+Signature; use crate::utils::{ build_siginfo, load_gbassembly_info,
+parse_params_str, GBAssemblyData, GenBankFileType, }; use reqwest::Url; async
+fn find_genome_directory( client: &Client, db: &str, number_path: &str,
+accession: &str, acc_number: &str, version: &str, ) -> Result<(Url, String)>
+{ let base_url = format!( "https://ftp.ncbi.nlm.nih.gov/genomes/all/{}/{}", db,
+number_path ); let directory_response = client.get(&base_url).send().await?; if
+!directory_response.status().is_success() { return Err(anyhow!( "Failed to open
+genome directory: HTTP {}, {}", directory_response.status(), directory_response
+.status() .canonical_reason() .unwrap_or("Unknown reason") )); } let text =
+directory_response.text().await?; let link_regex = Regex::new(r#"
++)/""#)?; for cap in link_regex.captures_iter(&text) { let name = ∩[1]; // Use
+acc numerical identifier and version as expected pattern let expected_pattern =
+format!("{}.{}", acc_number, version); // Check if directory name contains
+contains the right acc number and version if name.contains(&expected_pattern)
+{ let url = format!("{}/{}", base_url, name).parse()?; return Ok((url,
+name.to_string())); } } Err(anyhow!( "No matching directory found for accession
+{}", accession )) } async fn fetch_genbank_filename( client: &Client,
+accession: &str, url: Option, ) -> Result<(Url, String)> { let (db, acc) =
+accession .trim() .split_once('_') .ok_or_else(|| anyhow!("Invalid accession
+format"))?; let (acc_number, version) = acc.split_once('.').unwrap_or((acc,
+"1")); let number_path = acc_number .chars() .collect::
 _>>() .chunks(3) .map(|chunk| chunk.iter().collect::()) .collect::
-_>>() .join("/"); let base_url = format!( "https://ftp.ncbi.nlm.nih.gov/
-genomes/all/{}/{}", db, number_path ); let directory_response = client.get
-(&base_url).send().await; match directory_response { Ok(response) => { if
-!response.status().is_success() { return Err(anyhow!( "Failed to open genome
-directory: HTTP {}, {}", response.status(), response .status()
-.canonical_reason() .unwrap_or("Unknown reason") )); } let text = response.text
-().await?; let link_regex = Regex::new(r#"
-*)""#)?; for cap in link_regex.captures_iter(&text) { let name = ∩[1]; let
-clean_name = if name.ends_with('/') { name.strip_suffix('/').unwrap() } else
-{ name }; if clean_name.starts_with(db) && clean_name .split('_') .nth(1)
-.map_or(false, |x| x.starts_with(number)) { return Ok((format!("{}/{}",
-base_url, clean_name), clean_name.into())); } } Err(anyhow!( "No matching
-directory found for accession {}", accession )) } Err(e) => { // eprintln!
-("HTTP request failed for accession {}: {}", accession, e); Err(anyhow!( "HTTP
-request failed for accession {}: {}", accession, e )) } } } async fn
-download_and_parse_md5(client: &Client, url: &str) -> Result
-String, String>> { let response = client .get(url) .send() .await .context
-("Failed to send request")?; let content = response .text() .await .context
-("Failed to download MD5 checksum file")?; let mut checksums = HashMap::new();
-// Iterate over each line in the checksum file for line in content.lines()
-{ let parts: Vec<&str> = line.splitn(2, ' ').collect(); if parts.len() == 2 { /
-/ Trim the filename to remove any leading " ./" if present let filename = parts
-[1].trim_start_matches(" ./"); // remove any ' ', '.', '/' from front
-checksums.insert(filename.to_string(), parts[0].to_string()); } else { return
-Err(anyhow!( "Invalid checksum line format in URL {}: {}", url, line )); } } Ok
-(checksums) } // download and return data directly instead of saving to file
-async fn download_with_retry( client: &Client, url: &str, expected_md5:
-Option<&str>, retry_count: u32, ) -> Result
+_>>() .join("/"); let (url, name) = if let Some(url) = url { let url_parts:
+Vec<&str> = url .path_segments() .ok_or_else(|| anyhow!("Failed to extract path
+segments from URL"))? .collect(); let name = url_parts .last() .ok_or_else(||
+anyhow!("Failed to extract name from URL"))? .to_string(); (url, name) } else
+{ find_genome_directory(client, db, &number_path, accession, acc_number,
+version).await? }; Ok((url, name)) } async fn download_and_parse_md5(client:
+&Client, url: &Url) -> Result
+String, String>> { let response = client .get(url.clone()) .send() .await
+.context("Failed to send request")?; let content = response .text() .await
+.context("Failed to download MD5 checksum file")?; let mut checksums =
+HashMap::new(); // Iterate over each line in the checksum file for line in
+content.lines() { let parts: Vec<&str> = line.splitn(2, ' ').collect(); if
+parts.len() == 2 { // Trim the filename to remove any leading " ./" if present
+let filename = parts[1].trim_start_matches(" ./"); // remove any ' ', '.', '/
+' from front checksums.insert(filename.to_string(), parts[0].to_string()); }
+else { return Err(anyhow!( "Invalid checksum line format in URL {}: {}", url,
+line )); } } Ok(checksums) } // download and return data directly instead of
+saving to file async fn download_with_retry( client: &Client, url: &Url,
+expected_md5: Option<&str>, retry_count: u32, ) -> Result
 u8>> { let mut attempts = retry_count; let mut last_error: Option = None; while
-attempts > 0 { let response = client.get(url).send().await; match response { Ok
-(resp) if resp.status().is_success() => { let data = resp .bytes() .await
-.context("Failed to read bytes from response")?; if let Some(md5) =
+attempts > 0 { let response = client.get(url.clone()).send().await; match
+response { Ok(resp) if resp.status().is_success() => { let data = resp .bytes()
+.await .context("Failed to read bytes from response")?; if let Some(md5) =
 expected_md5 { let computed_hash = format!("{:x}", md5::compute(&data)); if
 computed_hash == md5 { return Ok(data.to_vec()); } else { last_error = Some
 (anyhow!( "MD5 hash does not match. Expected: {}, Found: {}", md5,
 computed_hash )); } } else { return Ok(data.to_vec()); // If no expected MD5 is
 provided, just return the data } } Ok(resp) => { last_error = Some(anyhow!
 ( "Server error status code {}: {}. Retrying...", resp.status(), url )); } Err
 (e) => { last_error = Some(anyhow!("Failed to download file: {}. Error: {}.",
@@ -79,43 +71,43 @@
 record")?; sigs.iter_mut().for_each(|sig| { if !set_name { sig.set_name(&name);
 sig.set_filename(&filename); }; if moltype == "protein" { sig.add_protein
 (&record.seq()) .expect("Failed to add protein"); } else { sig.add_sequence
 (&record.seq(), true) .expect("Failed to add sequence"); // if not force,
 panics with 'N' in dna sequence } }); if !set_name { set_name = true; } }
 Result::
 Signature>, anyhow::Error>::Ok(sigs) }) .await? } pub struct FailedDownload
-{ accession: String, name: String, url: String, moltype: String, } #[allow
+{ accession: String, name: String, url: Option, moltype: String, } #[allow
 (clippy::too_many_arguments)] async fn dl_sketch_accession( client: &Client,
-accession: String, name: String, location: &PathBuf, retry: Option,
-keep_fastas: bool, dna_sigs: Vec, prot_sigs: Vec, genomes_only: bool,
-proteomes_only: bool, download_only: bool, ) -> Result<(Vec, Vec)> { let
-retry_count = retry.unwrap_or(3); // Default retry count let mut sigs = Vec::::
-new(); let mut failed = Vec::::new(); // keep track of any accessions for which
-we fail to find URLs let (base_url, full_name) = match fetch_genbank_filename
-(client, accession.as_str()).await { Ok(result) => result, Err(_err) => { /
+accinfo: GBAssemblyData, location: &PathBuf, retry: Option, keep_fastas: bool,
+dna_sigs: Vec, prot_sigs: Vec, genomes_only: bool, proteomes_only: bool,
+download_only: bool, ) -> Result<(Vec, Vec)> { let retry_count =
+retry.unwrap_or(3); // Default retry count let mut sigs = Vec::::new(); let mut
+failed = Vec::::new(); let name = accinfo.name; let accession =
+accinfo.accession; // keep track of any accessions for which we fail to find
+URLs let (base_url, full_name) = match fetch_genbank_filename(client,
+accession.as_str(), accinfo.url).await { Ok(result) => result, Err(_err) => { /
 / Add accession to failed downloads with each moltype if !proteomes_only { let
 failed_download_dna = FailedDownload { accession: accession.clone(), name:
-name.clone(), url: "".to_string(), moltype: "dna".to_string(), }; failed.push
+name.clone(), url: None, moltype: "dna".to_string(), }; failed.push
 (failed_download_dna); } if !genomes_only { let failed_download_protein =
-FailedDownload { accession: accession.clone(), name: name.clone(), url:
-"".to_string(), moltype: "protein".to_string(), }; failed.push
-(failed_download_protein); } return Ok((sigs, failed)); } }; let md5sum_url =
-GenBankFileType::Checksum.url(&base_url, &full_name); let checksums = match
-download_and_parse_md5(client, &md5sum_url).await { Ok(cs) => cs, Err(e) =>
-{ return Err(e); } }; let mut file_types = vec![ GenBankFileType::Genomic,
-GenBankFileType::Protein, // GenBankFileType::AssemblyReport, ]; if
-genomes_only { file_types = vec![GenBankFileType::Genomic]; } else if
-proteomes_only { file_types = vec![GenBankFileType::Protein]; } for file_type
-in &file_types { let url = file_type.url(&base_url, &full_name); let
-expected_md5 = checksums.get(&file_type.server_filename(&full_name)); // let
-checksum = checksums let data = match download_with_retry(client, &url,
-expected_md5.map(|x| x.as_str()), retry_count) .await { Ok(data) => data, Err
-(_err) => { // here --> keep track of accession errors + filetype let
-failed_download = FailedDownload { accession: accession.clone(), name:
-name.clone(), url: url.clone(), moltype: file_type.moltype(), }; failed.push
+FailedDownload { accession: accession.clone(), name: name.clone(), url: None,
+moltype: "protein".to_string(), }; failed.push(failed_download_protein); }
+return Ok((sigs, failed)); } }; let md5sum_url = GenBankFileType::Checksum.url
+(&base_url, &full_name); let checksums = match download_and_parse_md5(client,
+&md5sum_url).await { Ok(cs) => cs, Err(e) => { return Err(e); } }; let mut
+file_types = vec![ GenBankFileType::Genomic, GenBankFileType::Protein, /
+/ GenBankFileType::AssemblyReport, ]; if genomes_only { file_types = vec!
+[GenBankFileType::Genomic]; } else if proteomes_only { file_types = vec!
+[GenBankFileType::Protein]; } for file_type in &file_types { let url =
+file_type.url(&base_url, &full_name); let expected_md5 = checksums.get
+(&file_type.server_filename(&full_name)); let data = match download_with_retry
+(client, &url, expected_md5.map(|x| x.as_str()), retry_count) .await { Ok(data)
+=> data, Err(_err) => { // here --> keep track of accession errors + filetype
+let failed_download = FailedDownload { accession: accession.clone(), name:
+name.clone(), url: Some(url), moltype: file_type.moltype(), }; failed.push
 (failed_download); continue; } }; let file_name = file_type.filename_to_write
 (&accession); if keep_fastas { let path = location.join(&file_name); fs::write
 (&path, &data).context("Failed to write data to file")?; } if !download_only
 { // sketch data match file_type { GenBankFileType::Genomic => sigs.extend
 ( sketch_data( name.clone(), file_name.clone(), data, dna_sigs.clone(),
 "dna".to_string(), ) .await?, ), GenBankFileType::Protein => { sigs.extend
 ( sketch_data( name.clone(), file_name.clone(), data, prot_sigs.clone(),
@@ -136,116 +128,129 @@
 (|e| anyhow!("Error creating gzip writer: {}", e))?; gz_writer.write_all
 (&json_bytes)?; // .map_err(|e| anyhow!("Error writing gzip data: {}", e))?; }
 buffer.into_inner() }; let now = Utc::now(); let builder = ZipEntryBuilder::new
 (sig_filename.into(), Compression::Stored) .last_modification_date
 (ZipDateTime::from_chrono(&now)); zip_writer .write_entry_whole(builder,
 &gzipped_buffer) .await .map_err(|e| anyhow!("Error writing zip entry: {}", e))
 } pub fn sigwriter_handle( mut recv_sigs: tokio::sync::mpsc::Receiver
-Signature>>, output_sigs: String, error_sender: tokio::sync::mpsc::Sender, ) -
+Signature>>, output_sigs: Option, error_sender: tokio::sync::mpsc::Sender, ) -
 > tokio::task::JoinHandle<()> { tokio::spawn(async move { let mut
 md5sum_occurrences = HashMap::new(); let mut manifest_rows = Vec::new(); let
-mut wrote_sigs = false; let outpath: PathBuf = output_sigs.into(); let file =
-match File::create(&outpath).await { Ok(file) => file, Err(e) => { let error =
-anyhow::Error::new(e).context("Failed to create file at specified path"); let _
-= error_sender.send(error).await; // Send the error through the channel return;
-// Simply exit the task as error handling is managed elsewhere } }; let mut
-zip_writer = ZipFileWriter::with_tokio(file); while let Some(sigs) =
-recv_sigs.recv().await { for sig in sigs { match write_sig( &sig, &mut
-md5sum_occurrences, &mut manifest_rows, &mut zip_writer, ) .await { Ok(_) =>
-wrote_sigs = true, Err(e) => { let error = e.context("Error processing
-signature"); if (error_sender.send(error).await).is_err() { return; // Exit on
-failure to send error } } } } } if wrote_sigs { println!("Writing manifest");
-let manifest_filename = "SOURMASH-MANIFEST.csv".to_string(); let manifest:
-Manifest = manifest_rows.clone().into(); let mut manifest_buffer = Vec::new();
-manifest .to_writer(&mut manifest_buffer) .expect("Failed to serialize
-manifest"); // Handle this more gracefully in production let now = Utc::now();
-let builder = ZipEntryBuilder::new(manifest_filename.into(), Compression::
-Stored) .last_modification_date(ZipDateTime::from_chrono(&now)); if let Err(e)
-= zip_writer .write_entry_whole(builder, &manifest_buffer) .await { let error =
-anyhow::Error::new(e).context("Failed to write manifest to ZIP"); let _ =
-error_sender.send(error).await; return; } if let Err(e) = zip_writer.close
-().await { let error = anyhow::Error::new(e).context("Failed to close ZIP
-file"); let _ = error_sender.send(error).await; return; } } else { let error =
-anyhow::Error::new(std::io::Error::new( std::io::ErrorKind::Other, "No
-signatures written", )); let _ = error_sender.send(error).await; // Send error
-about no signatures written } drop(error_sender); }) } pub fn failures_handle
-( failed_csv: String, mut recv_failed: tokio::sync::mpsc::Receiver,
-error_sender: tokio::sync::mpsc::Sender, // Additional parameter for error
-channel ) -> tokio::task::JoinHandle<()> { tokio::spawn(async move { match
-File::create(&failed_csv).await { Ok(file) => { let mut writer = BufWriter::new
-(file); // Attempt to write CSV headers if let Err(e) = writer.write_all
-(b"accession,name,moltype,url\n").await { let error = Error::new(e).context
-("Failed to write headers"); let _ = error_sender.send(error).await; return; /
-/ Exit the task early after reporting the error } while let Some(FailedDownload
-{ accession, name, moltype, url, }) = recv_failed.recv().await { let record =
-format!("{},{},{},{}\n", accession, name, moltype, url); // Attempt to write
-each record if let Err(e) = writer.write_all(record.as_bytes()).await { let
-error = Error::new(e).context("Failed to write record"); let _ =
-error_sender.send(error).await; continue; // Optionally continue to try to
-write next records } } // Attempt to flush the writer if let Err(e) =
-writer.flush().await { let error = Error::new(e).context("Failed to flush
-writer"); let _ = error_sender.send(error).await; } } Err(e) => { let error =
-Error::new(e).context("Failed to create file"); let _ = error_sender.send
-(error).await; } } drop(error_sender); }) } pub fn error_handler( mut
-recv_errors: tokio::sync::mpsc::Receiver, error_flag: Arc, ) -> tokio::task::
-JoinHandle<()> { tokio::spawn(async move { while let Some(error) =
-recv_errors.recv().await { eprintln!("Error: {}", error); if error.to_string
-().contains("No signatures written") { error_flag.store(true, Ordering::
-SeqCst); break; } } }) } #[tokio::main] #[allow(clippy::too_many_arguments)]
-pub async fn download_and_sketch( py: Python, input_csv: String, output_sigs:
+mut wrote_sigs = false; if let Some(outpath) = output_sigs { let outpath:
+PathBuf = outpath.into(); let file = match File::create(&outpath).await { Ok
+(file) => file, Err(e) => { let error = anyhow::Error::new(e).context("Failed
+to create file at specified path"); let _ = error_sender.send(error).await; /
+/ Send the error through the channel return; // Simply exit the task as error
+handling is managed elsewhere } }; let mut zip_writer = ZipFileWriter::
+with_tokio(file); while let Some(sigs) = recv_sigs.recv().await { for sig in
+sigs { match write_sig( &sig, &mut md5sum_occurrences, &mut manifest_rows, &mut
+zip_writer, ) .await { Ok(_) => wrote_sigs = true, Err(e) => { let error =
+e.context("Error processing signature"); if (error_sender.send
+(error).await).is_err() { return; // Exit on failure to send error } } } } } if
+wrote_sigs { println!("Writing manifest"); let manifest_filename = "SOURMASH-
+MANIFEST.csv".to_string(); let manifest: Manifest = manifest_rows.clone().into
+(); let mut manifest_buffer = Vec::new(); manifest .to_writer(&mut
+manifest_buffer) .expect("Failed to serialize manifest"); // Handle this more
+gracefully in production let now = Utc::now(); let builder = ZipEntryBuilder::
+new(manifest_filename.into(), Compression::Stored) .last_modification_date
+(ZipDateTime::from_chrono(&now)); if let Err(e) = zip_writer .write_entry_whole
+(builder, &manifest_buffer) .await { let error = anyhow::Error::new(e).context
+("Failed to write manifest to ZIP"); let _ = error_sender.send(error).await;
+return; } if let Err(e) = zip_writer.close().await { let error = anyhow::
+Error::new(e).context("Failed to close ZIP file"); let _ = error_sender.send
+(error).await; return; } } else { let error = anyhow::Error::new(std::io::
+Error::new( std::io::ErrorKind::Other, "No signatures written", )); let _ =
+error_sender.send(error).await; // Send error about no signatures written } }
+drop(error_sender); // should be dropped automatically as it goes out of scope,
+but just in case }) } pub fn failures_handle( failed_csv: String, mut
+recv_failed: tokio::sync::mpsc::Receiver, error_sender: tokio::sync::mpsc::
+Sender, // Additional parameter for error channel ) -> tokio::task::JoinHandle<
+()> { tokio::spawn(async move { match File::create(&failed_csv).await { Ok
+(file) => { let mut writer = BufWriter::new(file); // Attempt to write CSV
+headers if let Err(e) = writer.write_all(b"accession,name,moltype,url\n").await
+{ let error = Error::new(e).context("Failed to write headers"); let _ =
+error_sender.send(error).await; return; // Exit the task early after reporting
+the error } while let Some(FailedDownload { accession, name, moltype, url, }) =
+recv_failed.recv().await { let record = format!("{},{},{},{:?}\n", accession,
+name, moltype, url); // Attempt to write each record if let Err(e) =
+writer.write_all(record.as_bytes()).await { let error = Error::new(e).context
+("Failed to write record"); let _ = error_sender.send(error).await; continue; /
+/ Optionally continue to try to write next records } } // Attempt to flush the
+writer if let Err(e) = writer.flush().await { let error = Error::new(e).context
+("Failed to flush writer"); let _ = error_sender.send(error).await; } } Err(e)
+=> { let error = Error::new(e).context("Failed to create file"); let _ =
+error_sender.send(error).await; } } drop(error_sender); }) } pub fn
+error_handler( mut recv_errors: tokio::sync::mpsc::Receiver, error_flag: Arc, )
+-> tokio::task::JoinHandle<()> { tokio::spawn(async move { while let Some
+(error) = recv_errors.recv().await { eprintln!("Error: {}", error); if
+error.to_string().contains("No signatures written") { error_flag.store(true,
+Ordering::SeqCst); break; } } }) } #[tokio::main] #[allow(clippy::
+too_many_arguments)] pub async fn download_and_sketch( py: Python, input_csv:
 String, param_str: String, failed_csv: String, retry_times: u32,
 fasta_location: String, keep_fastas: bool, genomes_only: bool, proteomes_only:
-bool, download_only: bool, ) -> Result<(), anyhow::Error> { // if sig output
-doesn't end in zip, bail if Path::new(&output_sigs) .extension() .map_or(true,
-|ext| ext != "zip") { bail!("Output must be a zip file."); } // set up fasta
-download path let download_path = PathBuf::from(fasta_location); if
+bool, download_only: bool, output_sigs: Option, ) -> Result<(), anyhow::Error>
+{ // if sig output provided but doesn't end in zip, bail if let Some(ref
+output_sigs) = output_sigs { if Path::new(&output_sigs) .extension() .map_or
+(true, |ext| ext != "zip") { bail!("Output must be a zip file."); } } // set up
+fasta download path let download_path = PathBuf::from(fasta_location); if
 !download_path.exists() { create_dir_all(&download_path)?; } // create
 channels. buffer size here is 4 b/c we can do 3 downloads simultaneously let
 (send_sigs, recv_sigs) = tokio::sync::mpsc::channel::
 Signature>>(4); let (send_failed, recv_failed) = tokio::sync::mpsc::channel::
-(4); // // Error channel for handling task errors let (error_sender,
-error_receiver) = tokio::sync::mpsc::channel::(1); // // // Set up collector/
-writing tasks let mut handles = Vec::new(); let sig_handle = sigwriter_handle
+(4); // Error channel for handling task errors let (error_sender,
+error_receiver) = tokio::sync::mpsc::channel::(1); // Set up collector/writing
+tasks let mut handles = Vec::new(); let sig_handle = sigwriter_handle
 (recv_sigs, output_sigs, error_sender.clone()); let failures_handle =
 failures_handle(failed_csv, recv_failed, error_sender.clone()); let
 critical_error_flag = Arc::new(AtomicBool::new(false)); let error_handle =
 error_handler(error_receiver, critical_error_flag.clone()); handles.push
-(sig_handle); handles.push(failures_handle); handles.push(error_handle); // /
+(sig_handle); handles.push(failures_handle); handles.push(error_handle); /
 / Worker tasks let semaphore = Arc::new(Semaphore::new(3)); // Limiting
 concurrent downloads let client = Arc::new(Client::new()); // Open the file
 containing the accessions synchronously let (accession_info, n_accs) =
-load_accession_info(input_csv)?; if n_accs == 0 { bail!("No accessions to
-download and sketch.") } // // parse param string into params_vec, print error
-if fail let param_result = parse_params_str(param_str); let params_vec = match
+load_gbassembly_info(input_csv)?; if n_accs == 0 { bail!("No accessions to
+download and sketch.") } // parse param string into params_vec, print error if
+fail let param_result = parse_params_str(param_str); let params_vec = match
 param_result { Ok(params) => params, Err(e) => { bail!("Failed to parse params
 string: {}", e); } }; let dna_sig_templates = build_siginfo(&params_vec,
-"DNA"); let prot_sig_templates = build_siginfo(&params_vec, "protein"); /
+"DNA"); let prot_sig_templates = build_siginfo(&params_vec, "protein"); let mut
+genomes_only = genomes_only; let mut proteomes_only = proteomes_only; // Check
+if dna_sig_templates is empty and not keep_fastas if dna_sig_templates.is_empty
+() && !keep_fastas { eprintln!("No DNA signature templates provided, and --
+keep-fastas is not set."); proteomes_only = true; } // Check if
+protein_sig_templates is empty and not keep_fastas if
+prot_sig_templates.is_empty() && !keep_fastas { eprintln!("No protein signature
+templates provided, and --keep-fastas is not set."); genomes_only = true; } if
+genomes_only { if !download_only { eprintln!("Downloading and sketching genomes
+only."); } else { eprintln!("Downloading genomes only."); } } else if
+proteomes_only { if !download_only { eprintln!("Downloading and sketching
+proteomes only."); } else { eprintln!("Downloading proteomes only."); } } /
 / report every 1 percent (or every 1, whichever is larger) let
 reporting_threshold = std::cmp::max(n_accs / 100, 1); for (i, accinfo) in
 accession_info.into_iter().enumerate() { py.check_signals()?; // If
 interrupted, return an Err automatically let semaphore_clone = Arc::clone
 (&semaphore); let client_clone = Arc::clone(&client); let send_sigs =
 send_sigs.clone(); let send_failed = send_failed.clone(); let
 download_path_clone = download_path.clone(); // Clone the path for each task
 let send_errors = error_sender.clone(); let dna_sigs = dna_sig_templates.clone
 (); let prot_sigs = prot_sig_templates.clone(); tokio::spawn(async move { let
-_permit = semaphore_clone.acquire().await; // Report when the permit is
-available and processing begins if (i + 1) % reporting_threshold == 0 { let
+_permit = semaphore_clone.acquire().await; // progress report when the permit
+is available and processing begins if (i + 1) % reporting_threshold == 0 { let
 percent_processed = (((i + 1) as f64 / n_accs as f64) * 100.0).round();
 println!( "Starting accession {}/{} ({}%)", (i + 1), n_accs, percent_processed
 ); } // Perform download and sketch let result = dl_sketch_accession
-( &client_clone, accinfo.accession.clone(), accinfo.name.clone(),
-&download_path_clone, Some(retry_times), keep_fastas, dna_sigs, prot_sigs,
-genomes_only, proteomes_only, download_only, ) .await; match result { Ok((sigs,
-failed_downloads)) => { if let Err(e) = send_sigs.send(sigs).await { eprintln!
-("Failed to send signatures: {}", e); let _ = send_errors.send(e.into()).await;
-// Send the error through the channel } for fail in failed_downloads { if let
-Err(e) = send_failed.send(fail).await { eprintln!("Failed to send failed
-download info: {}", e); let _ = send_errors.send(e.into()).await; // Send the
-error through the channel } } } Err(e) => { let _ = send_errors.send(e).await;
-} } drop(send_errors); }); } // drop senders as we're done sending data drop
+( &client_clone, accinfo.clone(), &download_path_clone, Some(retry_times),
+keep_fastas, dna_sigs, prot_sigs, genomes_only, proteomes_only, download_only,
+) .await; match result { Ok((sigs, failed_downloads)) => { if !sigs.is_empty()
+{ if let Err(e) = send_sigs.send(sigs).await { eprintln!("Failed to send
+signatures: {}", e); let _ = send_errors.send(e.into()).await; // Send the
+error through the channel } } for fail in failed_downloads { if let Err(e) =
+send_failed.send(fail).await { eprintln!("Failed to send failed download info:
+{}", e); let _ = send_errors.send(e.into()).await; // Send the error through
+the channel } } } Err(e) => { let _ = send_errors.send(e).await; } } drop
+(send_errors); }); } // drop senders as we're done sending data drop
 (send_sigs); drop(send_failed); drop(error_sender); // Wait for all tasks to
 complete for handle in handles { if let Err(e) = handle.await { eprintln!
 ("Handle join error: {}.", e); } } // since the only critical error is not
 having written any sigs // check this here at end. Bail if we wrote expected
 sigs but wrote none. if critical_error_flag.load(Ordering::SeqCst) &
 !download_only { bail!("No signatures written, exiting."); } Ok(()) }
```

### Comparing `sourmash_plugin_directsketch-0.2.3/src/lib.rs` & `sourmash_plugin_directsketch-0.3.0/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -50,34 +50,34 @@
 #[pyfunction]
 #[allow(clippy::too_many_arguments)]
 fn do_gbsketch(
     py: Python,
     input_csv: String,
     param_str: String,
     failed_csv: String,
-    output_sigs: String,
     retry_times: u32,
     fasta_location: String,
     keep_fastas: bool,
     genomes_only: bool,
     proteomes_only: bool,
     download_only: bool,
+    output_sigs: Option<String>,
 ) -> anyhow::Result<u8> {
     match directsketch::download_and_sketch(
         py,
         input_csv,
-        output_sigs,
         param_str,
         failed_csv,
         retry_times,
         fasta_location,
         keep_fastas,
         genomes_only,
         proteomes_only,
         download_only,
+        output_sigs,
     ) {
         Ok(_) => Ok(0),
         Err(e) => {
             eprintln!("Error: {e}");
             Ok(1)
         }
     }
```

### Comparing `sourmash_plugin_directsketch-0.2.3/src/python/sourmash_plugin_directsketch/__init__.py` & `sourmash_plugin_directsketch-0.3.0/src/python/sourmash_plugin_directsketch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 class Download_and_Sketch_Assemblies(CommandLinePlugin):
     command = 'gbsketch'
     description = 'download and sketch GenBank assembly datasets'
 
     def __init__(self, p):
         super().__init__(p)
         p.add_argument('input_csv', help="a txt file or csv file containing accessions in the first column")
-        p.add_argument('-o', '--output', required=True,
+        p.add_argument('-o', '--output', default=None,
                        help='output zip file for the signatures')
         p.add_argument('-f', '--fastas',
                        help='Write fastas here', default = '.')
         p.add_argument('-k', '--keep-fastas', action='store_true',
                        help="write FASTA files in addition to sketching. Default: do not write FASTA files")
         p.add_argument('--download-only', help='just download genomes; do not sketch', action='store_true')
         p.add_argument('--failed',help='csv of failed accessions and download links (should be mostly protein).')
@@ -63,33 +63,40 @@
         if not args.param_string:
             args.param_string = ["k=31,scaled=1000"]
         notify(f"params: {args.param_string}")
 
         if args.download_only and not args.keep_fastas:
             notify("Error: '--download-only' requires '--keep-fastas'.")
             sys.exit(-1)
-            
+        if args.output is None and not args.download_only:
+            notify("Error: output signature zipfile is required if not using '--download-only'.")
+            sys.exit(-1)
 
         # convert to a single string for easier rust handling
         args.param_string = "_".join(args.param_string)
         # lowercase the param string
         args.param_string = args.param_string.lower()
 
         num_threads = set_thread_pool(args.cores)
 
         notify(f"downloading and sketching all accessions in '{args.input_csv} using {num_threads} threads")
 
         super().main(args)
         status = sourmash_plugin_directsketch.do_gbsketch(args.input_csv,
                                                            args.param_string,
                                                            args.failed,
-                                                           args.output,
                                                            args.retry_times,
                                                            args.fastas,
                                                            args.keep_fastas,
                                                            args.genomes_only,
                                                            args.proteomes_only,
-                                                           args.download_only)
+                                                           args.download_only,
+                                                           args.output)
         
         if status == 0:
-            notify(f"...gbsketch is done! Sigs in '{args.output}'. Fastas in '{args.fastas}'.")
+            notify("...gbsketch is done!")
+            if args.output is not None:
+                notify(f"Sigs in '{args.output}'.")
+            if args.keep_fastas:
+                notify(f"FASTAs in '{args.fastas}'.")
+
         return status
```

### Comparing `sourmash_plugin_directsketch-0.2.3/tests/sourmash_tst_utils.py` & `sourmash_plugin_directsketch-0.3.0/tests/sourmash_tst_utils.py`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.3/tests/test_gbsketch.py` & `sourmash_plugin_directsketch-0.3.0/tests/test_gbsketch.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 def test_gbsketch_simple(runtmp):
     acc_csv = get_test_data('acc.csv')
     output = runtmp.output('simple.zip')
     failed = runtmp.output('failed.csv')
 
-    sig1 = get_test_data('GCA_000175555.1.sig.gz')
+    sig1 = get_test_data('GCA_000175535.1.sig.gz')
     sig2 = get_test_data('GCA_000961135.2.sig.gz')
     sig3 = get_test_data('GCA_000961135.2.protein.sig.gz')
     ss1 = sourmash.load_one_signature(sig1, ksize=31)
     ss2 = sourmash.load_one_signature(sig2, ksize=31)
     # why does this need ksize =30 and not ksize = 10!???
     ss3 = sourmash.load_one_signature(sig3, ksize=30, select_moltype='protein')
 
@@ -42,30 +42,67 @@
     assert not runtmp.last_result.out # stdout should be empty
 
     idx = sourmash.load_file_as_index(output)
     sigs = list(idx.signatures())
 
     assert len(sigs) == 3
     for sig in sigs:
-        if 'GCA_000175555.1' in sig.name:
+        if 'GCA_000175535.1' in sig.name:
             assert sig.name == ss1.name
             assert sig.md5sum() == ss1.md5sum()
         elif 'GCA_000961135.2' in sig.name:
             assert sig.name == ss2.name
             if sig.minhash.moltype == 'DNA':
                 assert sig.md5sum() == ss2.md5sum()
             else:
                 assert sig.md5sum() == ss3.md5sum()
 
+
+def test_gbsketch_simple_url(runtmp):
+    acc_csv = get_test_data('acc-with-ftppath.csv')
+    output = runtmp.output('simple.zip')
+    failed = runtmp.output('failed.csv')
+
+    sig1 = get_test_data('GCA_000175535.1.sig.gz')
+    sig2 = get_test_data('GCA_000961135.2.sig.gz')
+    sig3 = get_test_data('GCA_000961135.2.protein.sig.gz')
+    ss1 = sourmash.load_one_signature(sig1, ksize=31)
+    ss2 = sourmash.load_one_signature(sig2, ksize=31)
+    # why does this need ksize =30 and not ksize = 10!???
+    ss3 = sourmash.load_one_signature(sig3, ksize=30, select_moltype='protein')
+
+    runtmp.sourmash('scripts', 'gbsketch', acc_csv, '-o', output,
+                    '--failed', failed, '-r', '1',
+                    '--param-str', "dna,k=31,scaled=1000", '-p', "protein,k=10,scaled=200")
+
+    assert os.path.exists(output)
+    assert not runtmp.last_result.out # stdout should be empty
+
+    idx = sourmash.load_file_as_index(output)
+    sigs = list(idx.signatures())
+
+    assert len(sigs) == 3
+    for sig in sigs:
+        if 'GCA_000175535.1' in sig.name:
+            assert sig.name == ss1.name
+            assert sig.md5sum() == ss1.md5sum()
+        elif 'GCA_000961135.2' in sig.name:
+            assert sig.name == ss2.name
+            if sig.minhash.moltype == 'DNA':
+                assert sig.md5sum() == ss2.md5sum()
+            else:
+                assert sig.md5sum() == ss3.md5sum()
+
+
 def test_gbsketch_genomes_only(runtmp):
     acc_csv = get_test_data('acc.csv')
     output = runtmp.output('simple.zip')
     failed = runtmp.output('failed.csv')
 
-    sig1 = get_test_data('GCA_000175555.1.sig.gz')
+    sig1 = get_test_data('GCA_000175535.1.sig.gz')
     sig2 = get_test_data('GCA_000961135.2.sig.gz')
     ss1 = sourmash.load_one_signature(sig1, ksize=31)
     ss2 = sourmash.load_one_signature(sig2, ksize=31)
 
     runtmp.sourmash('scripts', 'gbsketch', acc_csv, '-o', output,
                     '--failed', failed, '-r', '1', '--genomes-only',
                     '--param-str', "dna,k=31,scaled=1000", '-p', "protein,k=10,scaled=200")
@@ -74,15 +111,15 @@
     assert not runtmp.last_result.out # stdout should be empty
 
     idx = sourmash.load_file_as_index(output)
     sigs = list(idx.signatures())
 
     assert len(sigs) == 2
     for sig in sigs:
-        if 'GCA_000175555.1' in sig.name:
+        if 'GCA_000175535.1' in sig.name:
             assert sig.name == ss1.name
             assert sig.md5sum() == ss1.md5sum()
         elif 'GCA_000961135.2' in sig.name:
             assert sig.name == ss2.name
             assert sig.md5sum() == ss2.md5sum()
 
 
@@ -107,96 +144,159 @@
 
     assert len(sigs) == 1
     for sig in sigs:
         assert 'GCA_000961135.2' in sig.name
         assert sig.md5sum() == ss3.md5sum()
 
 
+def test_gbsketch_genomes_only_via_params(runtmp, capfd):
+    acc_csv = get_test_data('acc.csv')
+    output = runtmp.output('simple.zip')
+    failed = runtmp.output('failed.csv')
+
+    sig1 = get_test_data('GCA_000175535.1.sig.gz')
+    sig2 = get_test_data('GCA_000961135.2.sig.gz')
+    ss1 = sourmash.load_one_signature(sig1, ksize=31)
+    ss2 = sourmash.load_one_signature(sig2, ksize=31)
+
+    runtmp.sourmash('scripts', 'gbsketch', acc_csv, '-o', output,
+                    '--failed', failed, '-r', '1',
+                    '--param-str', "dna,k=31,scaled=1000")
+
+    assert os.path.exists(output)
+    assert not runtmp.last_result.out # stdout should be empty
+
+    idx = sourmash.load_file_as_index(output)
+    sigs = list(idx.signatures())
+    captured = capfd.readouterr()
+
+    assert len(sigs) == 2
+    for sig in sigs:
+        if 'GCA_000175535.1' in sig.name:
+            assert sig.name == ss1.name
+            assert sig.md5sum() == ss1.md5sum()
+        elif 'GCA_000961135.2' in sig.name:
+            assert sig.name == ss2.name
+            assert sig.md5sum() == ss2.md5sum()
+    assert 'No protein signature templates provided, and --keep-fastas is not set.' in captured.err
+    assert 'Downloading and sketching genomes only.' in captured.err
+
+
+def test_gbsketch_proteomes_only_via_params(runtmp, capfd):
+    acc_csv = get_test_data('acc.csv')
+    output = runtmp.output('simple.zip')
+    failed = runtmp.output('failed.csv')
+
+    sig3 = get_test_data('GCA_000961135.2.protein.sig.gz')
+    # why does this need ksize =30 and not ksize = 10!???
+    ss3 = sourmash.load_one_signature(sig3, ksize=30, select_moltype='protein')
+
+    runtmp.sourmash('scripts', 'gbsketch', acc_csv, '-o', output,
+                    '--failed', failed, '-r', '1',
+                    '--param-str', "protein,k=10,scaled=200")
+
+    assert os.path.exists(output)
+    assert not runtmp.last_result.out # stdout should be empty
+    print(runtmp.last_result.err)
+
+    idx = sourmash.load_file_as_index(output)
+    sigs = list(idx.signatures())
+    captured = capfd.readouterr()
+
+    assert len(sigs) == 1
+    for sig in sigs:
+        assert 'GCA_000961135.2' in sig.name
+        assert sig.md5sum() == ss3.md5sum()
+    assert 'No DNA signature templates provided, and --keep-fastas is not set.' in captured.err
+    assert 'Downloading and sketching proteomes only.' in captured.err
+
+
 def test_gbsketch_save_fastas(runtmp):
     acc_csv = get_test_data('acc.csv')
     output = runtmp.output('simple.zip')
     failed = runtmp.output('failed.csv')
     out_dir = runtmp.output('out_fastas')
 
 
-    sig1 = get_test_data('GCA_000175555.1.sig.gz')
+    sig1 = get_test_data('GCA_000175535.1.sig.gz')
     sig2 = get_test_data('GCA_000961135.2.sig.gz')
     sig3 = get_test_data('GCA_000961135.2.protein.sig.gz')
     ss1 = sourmash.load_one_signature(sig1, ksize=31)
     ss2 = sourmash.load_one_signature(sig2, ksize=31)
     # why does this need ksize =30 and not ksize = 10!???
     ss3 = sourmash.load_one_signature(sig3, ksize=30, select_moltype='protein')
 
     runtmp.sourmash('scripts', 'gbsketch', acc_csv, '-o', output,
                     '--failed', failed, '-r', '1', '--fastas', out_dir, '--keep-fastas',
                     '--param-str', "dna,k=31,scaled=1000", '-p', "protein,k=10,scaled=200")
 
     assert os.path.exists(output)
     assert not runtmp.last_result.out # stdout should be empty
     fa_files = os.listdir(out_dir)
-    assert set(fa_files) == set(['GCA_000175555.1_genomic.fna.gz', 'GCA_000961135.2_protein.faa.gz', 'GCA_000961135.2_genomic.fna.gz'])
+    assert set(fa_files) == set(['GCA_000175535.1_genomic.fna.gz', 'GCA_000961135.2_protein.faa.gz', 'GCA_000961135.2_genomic.fna.gz'])
 
     idx = sourmash.load_file_as_index(output)
     sigs = list(idx.signatures())
 
     assert len(sigs) == 3
     for sig in sigs:
-        if 'GCA_000175555.1' in sig.name:
+        if 'GCA_000175535.1' in sig.name:
             assert sig.name == ss1.name
             assert sig.md5sum() == ss1.md5sum()
         elif 'GCA_000961135.2' in sig.name:
             assert sig.name == ss2.name
             if sig.minhash.moltype == 'DNA':
                 assert sig.md5sum() == ss2.md5sum()
             else:
                 assert sig.md5sum() == ss3.md5sum()
 
-def test_gbsketch_download_only(runtmp):
+def test_gbsketch_download_only(runtmp, capfd):
     acc_csv = get_test_data('acc.csv')
     output = runtmp.output('simple.zip')
     failed = runtmp.output('failed.csv')
     out_dir = runtmp.output('out_fastas')
 
 
-    sig1 = get_test_data('GCA_000175555.1.sig.gz')
+    sig1 = get_test_data('GCA_000175535.1.sig.gz')
     sig2 = get_test_data('GCA_000961135.2.sig.gz')
     sig3 = get_test_data('GCA_000961135.2.protein.sig.gz')
     ss1 = sourmash.load_one_signature(sig1, ksize=31)
     ss2 = sourmash.load_one_signature(sig2, ksize=31)
     # why does this need ksize =30 and not ksize = 10!???
     ss3 = sourmash.load_one_signature(sig3, ksize=30, select_moltype='protein')
 
-    runtmp.sourmash('scripts', 'gbsketch', acc_csv, '-o', output, '--download-only',
+    runtmp.sourmash('scripts', 'gbsketch', acc_csv, '--download-only',
                     '--failed', failed, '-r', '1', '--fastas', out_dir, '--keep-fastas',
                     '--param-str', "dna,k=31,scaled=1000", '-p', "protein,k=10,scaled=200")
 
-    assert os.path.exists(output) # would be better if this didn't exist
     assert not runtmp.last_result.out # stdout should be empty
     fa_files = os.listdir(out_dir)
-    assert set(fa_files) == set(['GCA_000175555.1_genomic.fna.gz', 'GCA_000961135.2_protein.faa.gz', 'GCA_000961135.2_genomic.fna.gz'])
+    assert set(fa_files) == set(['GCA_000175535.1_genomic.fna.gz', 'GCA_000961135.2_protein.faa.gz', 'GCA_000961135.2_genomic.fna.gz'])
+    captured = capfd.readouterr()
+    assert "Failed to send signatures: channel closed" not in captured.err
    
 
 def test_gbsketch_bad_acc(runtmp):
     acc_csv = get_test_data('acc.csv')
     acc_mod = runtmp.output('acc_mod.csv')
     with open(acc_csv, 'r') as inF, open(acc_mod, 'w') as outF:
         lines = inF.readlines()
         for line in lines:
             # if this acc exist in line, copy it and write an extra line with an invalid accession
             outF.write(line)
             print(line)
-            if "GCA_000175555.1" in line:
-                mod_line = line.replace('GCA_000175555.1', 'GCA_0001755559.1')  # add extra digit - should not be valid
+            if "GCA_000175535.1" in line:
+                mod_line = line.replace('GCA_000175535.1', 'GCA_0001755559.1')  # add extra digit - should not be valid
                 print(mod_line)
                 outF.write(mod_line)
 
     output = runtmp.output('simple.zip')
     failed = runtmp.output('failed.csv')
 
-    sig1 = get_test_data('GCA_000175555.1.sig.gz')
+    sig1 = get_test_data('GCA_000175535.1.sig.gz')
     sig2 = get_test_data('GCA_000961135.2.sig.gz')
     sig3 = get_test_data('GCA_000961135.2.protein.sig.gz')
     ss1 = sourmash.load_one_signature(sig1, ksize=31)
     ss2 = sourmash.load_one_signature(sig2, ksize=31)
     # why does this need ksize =30 and not ksize = 10!???
     ss3 = sourmash.load_one_signature(sig3, ksize=30, select_moltype='protein')
 
@@ -222,15 +322,15 @@
             assert False, "Modified accession not found"
 
     idx = sourmash.load_file_as_index(output)
     sigs = list(idx.signatures())
 
     assert len(sigs) == 3
     for sig in sigs:
-        if 'GCA_000175555.1' in sig.name:
+        if 'GCA_000175535.1' in sig.name:
             assert sig.name == ss1.name
             assert sig.md5sum() == ss1.md5sum()
         elif 'GCA_000961135.2' in sig.name:
             assert sig.name == ss2.name
             if sig.minhash.moltype == 'DNA':
                 assert sig.md5sum() == ss2.md5sum()
             else:
@@ -247,49 +347,103 @@
                     '--failed', failed, '-r', '1',
                     '--param-str', "dna,k=31,scaled=1000", '-p', "protein,k=10,scaled=200")
         
     captured = capfd.readouterr()
     print(captured.err)
     assert "Error: No such file or directory" in captured.err
 
+
 def test_gbsketch_empty_accfile(runtmp, capfd):
     acc_csv = get_test_data('acc1.csv')
     with open(acc_csv, 'w') as file:
         file.write('')
     output = runtmp.output('simple.zip')
     failed = runtmp.output('failed.csv')
 
     with pytest.raises(utils.SourmashCommandFailed):
         runtmp.sourmash('scripts', 'gbsketch', acc_csv, '-o', output,
                     '--failed', failed, '-r', '1',
                     '--param-str', "dna,k=31,scaled=1000", '-p', "protein,k=10,scaled=200")
         
     captured = capfd.readouterr()
     print(captured.err)
-    assert "Error: No accessions to download and sketch." in captured.err
+    assert 'Error: Invalid column names in CSV file. Columns should be: ["accession", "name", "ftp_path"]' in captured.err
 
 
 def test_gbsketch_bad_acc_fail(runtmp, capfd):
     acc_csv = get_test_data('acc.csv')
     acc_mod = runtmp.output('acc_mod.csv')
     with open(acc_csv, 'r') as inF, open(acc_mod, 'w') as outF:
         lines = inF.readlines()
         outF.write(lines[0])  # write the header line
         for line in lines:
             # if this acc exist in line, copy it and write
-            if "GCA_000175555.1" in line:
-                mod_line = line.replace('GCA_000175555.1', 'GCA_0001755559.1')  # add extra digit - should not be valid
+            if "GCA_000175535.1" in line:
+                mod_line = line.replace('GCA_000175535.1', 'GCA_0001755559.1')  # add extra digit - should not be valid
                 print(mod_line)
                 outF.write(mod_line)
     
     output = runtmp.output('simple.zip')
     failed = runtmp.output('failed.csv')
 
     with pytest.raises(utils.SourmashCommandFailed):
         runtmp.sourmash('scripts', 'gbsketch', acc_mod, '-o', output,
                     '--failed', failed, '-r', '1',
                     '--param-str', "dna,k=31,scaled=1000")
         
     captured = capfd.readouterr()
     print(captured.out)
     print(captured.err)
-    assert "Error: No signatures written, exiting." in captured.err
+    assert "Error: No signatures written, exiting." in captured.err
+
+
+def test_gbsketch_version_bug(runtmp):
+    acc_csv = get_test_data('acc-version.csv')
+    output = runtmp.output('simple.zip')
+    failed = runtmp.output('failed.csv')
+
+    sig1 = get_test_data('GCA_000193795.2.sig.gz')
+    ss1 = sourmash.load_one_signature(sig1, ksize=31)
+
+    runtmp.sourmash('scripts', 'gbsketch', acc_csv, '-o', output,
+                    '--failed', failed, '-r', '1',
+                    '--param-str', "dna,k=31,scaled=1000")
+
+    assert os.path.exists(output)
+    assert not runtmp.last_result.out # stdout should be empty
+
+    idx = sourmash.load_file_as_index(output)
+    sigs = list(idx.signatures())
+
+    assert len(sigs) == 1
+    for sig in sigs:
+        assert sig.name == ss1.name == "GCA_000193795.2 Neisseria lactamica NS19 (b-proteobacteria) strain=NS19"
+        assert sig.md5sum() == ss1.md5sum() == "7ead366dcfed8e8ab938f771459c4e94"
+
+
+def test_gbsketch_cols_trailing_commas(runtmp, capfd):
+    acc_csv = get_test_data('acc-cols.csv')
+    output = runtmp.output('simple.zip')
+    failed = runtmp.output('failed.csv')
+
+    with pytest.raises(utils.SourmashCommandFailed):
+        runtmp.sourmash('scripts', 'gbsketch', acc_csv, '-o', output,
+                '--failed', failed, '-r', '1',
+                '--param-str', "dna,k=31,scaled=1000", '-p', "protein,k=10,scaled=200")
+        
+    captured = capfd.readouterr()
+    print(captured.err)
+    assert 'Error: CSV error: record 1 (line: 1, byte: 24): found record with 2 fields, but the previous record has 3 fields' in captured.err
+
+
+def test_gbsketch_missing_output(runtmp):
+    # no output sig zipfile provided but also not --download-only
+    acc_csv = runtmp.output('acc1.csv')
+    output = runtmp.output('simple.zip')
+    failed = runtmp.output('failed.csv')
+
+    with pytest.raises(utils.SourmashCommandFailed):
+        runtmp.sourmash('scripts', 'gbsketch', acc_csv,
+                    '--failed', failed, '-r', '1',
+                    '--param-str', "dna,k=31,scaled=1000")
+
+    assert "Error: output signature zipfile is required if not using '--download-only'." in runtmp.last_result.err
```

### Comparing `sourmash_plugin_directsketch-0.2.3/Cargo.lock` & `sourmash_plugin_directsketch-0.3.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1811,15 +1811,15 @@
  "vec-collections",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "sourmash_plugin_directsketch"
-version = "0.2.3"
+version = "0.3.0"
 dependencies = [
  "anyhow",
  "async_zip",
  "camino",
  "chrono",
  "csv",
  "futures",
```

### Comparing `sourmash_plugin_directsketch-0.2.3/pyproject.toml` & `sourmash_plugin_directsketch-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.3/PKG-INFO` & `sourmash_plugin_directsketch-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sourmash_plugin_directsketch
-Version: 0.2.3
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: sourmash >=4.8.5, <5
 Requires-Dist: pytest >=6.2.4, <8.3.0 ; extra == 'test'
 Requires-Dist: pytest-cov >=2.12, <6.0 ; extra == 'test'
 Requires-Dist: pytest-xdist ; extra == 'test'
@@ -29,23 +29,37 @@
 ## Installation
 
 ```
 pip install sourmash_plugin_directsketch
 ```
 
 ## Usage
+
+### Create an input file
+
 First, create a file, e.g. `acc.csv` with GenBank identifiers and sketch names.
 ```
-ident,name
-GCA_000961135.2,GCA_000961135.2 Candidatus Aramenus sulfurataquae isolate AZ1-45
-GCA_000175555.1,GCA_000175555.1 ACUK01000506.1 Saccharolobus solfataricus 98/2
+accession,name,ftp_path
+GCA_000961135.2,GCA_000961135.2 Candidatus Aramenus sulfurataquae isolate AZ1-45,
+GCA_000175555.1,GCA_000175555.1 ACUK01000506.1 Saccharolobus solfataricus 98/2,
 ```
-> Extra columns are ok, as long as the first two columns contain the identifier and sketch name
+> Three columns must be present: `accession`, `name`, and `ftp_path`. The `ftp_path` column can be empty, but no additional columns may be present.
+
+#### What is ftp_path?
+
+If you do not provide an `ftp_path`, `gbsketch` will use the accession to find the `ftp_path` for you.
+
+If you choose to provide it, `ftp_path` must be the `ftp_path` column from NCBI's assembly summary files.
+
+For reference:
+
+- example `ftp_path`: [https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/036/600/915/GCA_036600915.1_ASM3660091v1](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/036/600/915/GCA_036600915.1_ASM3660091v1)
+- bacteria assembly summary file: [https://ftp.ncbi.nih.gov/genomes/genbank/bacteria/assembly_summary.txt](https://ftp.ncbi.nih.gov/genomes/genbank/bacteria/assembly_summary.txt)
 
-Run:
+### Run:
 
 To run the test accession file at `tests/test-data/acc.csv`, run:
 ```
 sourmash scripts gbsketch tests/test-data/acc.csv -o test.zip -f out_fastas -k --failed test.failed.csv -p dna,k=21,k=31,scaled=1000,abund -p protein,k=10,scaled=100,abund -r 1
 ```
 
 Full Usage:
```

