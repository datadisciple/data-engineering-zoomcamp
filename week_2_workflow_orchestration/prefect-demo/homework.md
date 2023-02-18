Question 1: 447,770
```bash
prefect deployment run etl-parent-flow/docker-flow --params '{"months": [1], "color": "green", "year": 2020}'
```

Question 2: `0 5 1 * *`

Question 3: 14851920
refer to [el_gcs_to_bq.py](/flows/04_homework/el_gcs_to_bq.py)

Question 4: 88605
```bash
prefect deployment build week_2_workflow_orchestration/prefect-demo/flows/03_deployments/parameterized_flow.py:etl_parent_flow -n dtc-wk2hw4 --params='{"months": [11], "color": "green", "year": 2020}' -sb github/de-zoomcamp-week2-branch -a
```
^ trick here was to path the entire path from the root repo folder into the build otherwise prefect won't be able to find the flow

Question 5:
skipped — it's on setting up email or slack notifications for flow runs in prefect

Question 6: 8