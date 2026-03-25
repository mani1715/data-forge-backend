# TODO: Fix /api/upload endpoint in data_routes.py

## Approved Plan Steps (Breakdown):

### Step 1: ✅ Plan approved by user
### Step 2: Create this TODO.md ✅

### Step 3: Edit routes/data_routes.py ✅
- [x] Add debug prints after df load: "UPLOAD SUCCESS", "Rows:", df.shape[0], "Columns:", df.shape[1]
- [x] Override summary with hardcoded df.shape calculations (rows, columns, missing_values, duplicates)
- [x] Update jsonify response to EXACT structure: message, quality_score (float), summary, preview (df.head(20).to_dict()), chart_data or {}
- [x] Enhance except block: print("UPLOAD ERROR:", str(e))

### Step 4: Test endpoint
- [ ] Run server (if needed: python server.py or similar)
- [ ] curl -X POST http://localhost:8001/api/upload -F "file=@test.csv"
- [ ] Verify logs show debug prints
- [ ] Verify response has stable summary.rows structure

### Step 5: Complete task
- [ ] attempt_completion with results
