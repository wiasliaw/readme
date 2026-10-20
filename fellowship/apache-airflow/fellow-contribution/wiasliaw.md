# wiasliaw

- GitHub：https://github.com/wiasliaw

---

Month: September 2026
Summary: PR: 3（merged 1、open 2）, Code Review: 0, Issue Discussion: 1, Dev List: 0

PR:
- [Add time range filtering to the Gantt view](https://github.com/apache/airflow/pull/73555)（open，milestone Airflow 3.4.0，15 files，+558/-24）：Gantt view 新增 start/end date 時間範圍篩選（API + UI），解決重跑後時間軸被舊 try 拉長、短任務被壓扁的問題，closes [#63715](https://github.com/apache/airflow/issues/63715)
- [Keep the URL scheme out of path masking in airflow info --anonymize](https://github.com/apache/airflow/pull/73599)（merged，Airflow 3.3.3，2 files，+41/-2）：修正 `airflow info --anonymize` 在 OS username 為 scheme 子字串時會破壞輸出的 bug，只遮罩 scheme 之後的部分並補上參數化測試
- [Normalize empty project id in credential config file branch](https://github.com/apache/airflow/pull/73886)（open，2 files，+15）：Google provider credential config file 分支在 project id 為 `None` 時正規化為 `""`，與 ADC / IdP 分支及型別註記一致，附單元測試

Issue Discussion:
- [#63715 Add a time range selector for the Gantt view](https://github.com/apache/airflow/issues/63715)：整理兩種篩選語意（單一時間窗 vs. 各欄位範圍）與 x 軸 clamp 行為的取捨，向 maintainer 確認設計方向
