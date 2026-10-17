# Relatos de bugs

Registros históricos de outubro de 2026, transcritos do relatório de estudo. IDs preservados para rastreabilidade. Estes registros não representam uma nova reprodução nem confirmam que as falhas persistem hoje.

As evidências não estão incluídas nesta versão pública. Não há necessidade de acessar o Jira para ler os relatos abaixo.

## HUNT-3 — Location search returns no results and blocks candidate profile setup

**Plataforma:** iOS  
**Severidade:** Major · **Prioridade:** High

**Ambiente registrado:** iPhone 15 Plus; iOS 26.6.2; Huntd 1.2.6.22

**Pré-condições:** Owned candidate account; Role stage completed.

**Passos:**

1. Open Profile > Candidate.
2. Complete Role.
3. Fill Expectations.
4. Search Brazil, São Paulo and London.
5. Try Save and continue.

**Resultado obtido:** Location search returns no results and profile setup cannot continue, including reported Remote attempt.

**Resultado esperado:** Supported location matches appear and valid setup can continue.

## HUNT-5 — Candidates page fails to load after clicking View candidates

**Plataforma:** Web  
**Severidade:** Major · **Prioridade:** High

**Ambiente registrado:** Windows 10 Pro 22H2 build 19045.6466; Chrome 154.0.8037.98 reported, updated version pending

**Pré-condições:** Owned newly created recruiter account.

**Passos:**

1. Complete recruiter onboarding.
2. Select View candidates.
3. Refresh.

**Resultado obtido:** Client-side exception displayed; after refresh, Luana reports error 500.

**Resultado esperado:** Candidate list or meaningful empty state loads.

## HUNT-21 — Password recovery email is not received after confirmation

**Plataforma:** iOS  
**Severidade:** Major · **Prioridade:** High

**Ambiente registrado:** iPhone 15 Plus / iOS 26.6.2 / Huntd 1.2.6.22

**Pré-condições:** Owned registered account.

**Passos:**

1. Open password recovery from the app.
2. Submit the registered email.
3. Check inbox and spam. 

**Resultado obtido:** The app opens a web page displaying “We sent you a link to reset your password by email”, but no recovery email is received in the inbox or spam folder.

**Resultado esperado:** A recovery email arrives and provides a usable password reset link.

## HUNT-22 — Desired position and Employment options are cleared after returning from Expectations

**Plataforma:** iOS  
**Severidade:** Major · **Prioridade:** High

**Ambiente registrado:** iPhone 15 Plus / iOS 26.6.2 / Huntd 1.2.6.22

**Pré-condições:** Owned candidate account; Role fields populated.

**Passos:**

1. Fill Role fields.
2. Continue to Expectations.
3. Return using the app back arrow.

**Resultado obtido:** Desired position and Employment options are cleared after returning from Expectations using the app's back arrow.

**Resultado esperado:** Previously entered Role values remain selected.

## HUNT-23 — Testimonials carousel shows fewer than 10 distinct testimonials

**Plataforma:** Web  
**Severidade:** Minor · **Prioridade:** Medium

**Ambiente registrado:** Windows 10 Pro 22H2; Chrome 154.0.8037.98 (64-bit)

**Pré-condições:** Open Huntd web landing page.

**Passos:**

1. Open the Huntd web landing page.
2. Scroll to the testimonials section.
3. Review all carousel testimonials.
4. Count only distinct testimonials, excluding duplicate slides.

**Resultado obtido:** Only 5 distinct testimonials are available; other carousel slides are duplicates.

**Resultado esperado:** At least 10 distinct testimonials should be displayed.

## HUNT-24 — Candidate experience is displayed in reverse chronological order

**Plataforma:** Web  
**Severidade:** Minor · **Prioridade:** Medium

**Ambiente registrado:** Windows 10 Pro 22H2; Chrome 154.0.8037.98 (64-bit)

**Pré-condições:** Recruiter account; candidate with multiple work experiences.

**Passos:**

1. Log in as recruiter.
2. Open Candidates.
3. Open a candidate with multiple experiences.
4. Review experience order.

**Resultado obtido:** Experience entries are displayed from newest to oldest.

**Resultado esperado:** Experience entries should be displayed from oldest to newest.

## HUNT-25 — Technology filter clears selected option instead of applying it

**Plataforma:** Web  
**Severidade:** Major · **Prioridade:** High

**Ambiente registrado:** Windows 10 Pro 22H2; Chrome 154.0.8037.98 (64-bit)

**Pré-condições:** Activated recruiter account.

**Passos:**

1. Log in as recruiter.
2. Open Candidates.
3. Open technology filter.
4. Search Solidity.
5. Select Solidity.
6. Observe field and results.

**Resultado obtido:** The selected technology is cleared and the filter is not applied.

**Resultado esperado:** Solidity should remain selected and filter the candidate list.

## HUNT-26 — Location filter returns no selectable options

**Plataforma:** Web  
**Severidade:** Major · **Prioridade:** High

**Ambiente registrado:** Windows 10 Pro 22H2; Chrome 154.0.8037.98 (64-bit)

**Pré-condições:** Activated recruiter account.

**Passos:**

1. Log in as recruiter.
2. Open Candidates.
3. Open location filter.
4. Search Brazil.
5. Repeat with London.

**Resultado obtido:** No selectable location options are returned.

**Resultado esperado:** Valid locations should appear and be selectable as filters.

## HUNT-27 — Recruiter onboarding does not complete as expected

**Plataforma:** Web  
**Severidade:** Major · **Prioridade:** High

**Ambiente registrado:** Windows 10 Pro 22H2; Chrome 154.0.8037.98 (64-bit)

**Pré-condições:** Owned recruiter account.

**Passos:**

1. Start recruiter onboarding.
2. Fill required recruiter information.
3. Continue through role, technologies, salary, experience, English and location.
4. Attempt completion.

**Resultado obtido:** The recruiter onboarding flow does not complete according to the expected flow.

**Resultado esperado:** All required onboarding steps should complete and open the Candidates page.

## HUNT-28 — Candidate onboarding does not fully match expected requirements

**Plataforma:** Web  
**Severidade:** Major · **Prioridade:** High

**Ambiente registrado:** Windows 10 Pro 22H2; Chrome 154.0.8037.98 (64-bit)

**Pré-condições:** Owned candidate account.

**Passos:**

1. Complete Role.
2. Complete Expectations.
3. Add experience.
4. Complete Bio and Contacts.
5. Submit profile.
6. Review fields and completion messages.

**Resultado obtido:** Expected requirements are inconsistent or missing, including EUR salary option, experience date handling and activation/review information.

**Resultado esperado:** All required fields/options should be available, saved correctly and expected review information displayed.

## HUNT-29 — Password recovery email is not received

**Plataforma:** Web  
**Severidade:** Major · **Prioridade:** High

**Ambiente registrado:** Windows 10 Pro 22H2; Chrome 154.0.8037.98 (64-bit)

**Pré-condições:** Owned registered account.

**Passos:**

1. Open sign-in page.
2. Click Forgot password.
3. Enter a valid registered email.
4. Submit request.
5. Check inbox and spam.

**Resultado obtido:** The recovery request is accepted, but no password reset email is received.

**Resultado esperado:** A password reset email should be delivered to the registered email address.

## HUNT-30 — Send offer action is missing in recruiter chat

**Plataforma:** Web  
**Severidade:** Major · **Prioridade:** High

**Ambiente registrado:** Windows 10 Pro 22H2; Chrome 154.0.8037.98 (64-bit)

**Pré-condições:** Recruiter account with an existing candidate conversation.

**Passos:**

1. Log in as recruiter.
2. Open a candidate conversation.
3. Inspect chat actions/status controls.
4. Look for Send offer.

**Resultado obtido:** Hire candidate, Reject candidate, Archive/Unarchive and Delete are available, but Send offer is missing.

**Resultado esperado:** Recruiter should be able to send a job offer from the chat.

## HUNT-31 — Favourite chat action is missing for candidate and recruiter

**Plataforma:** Web  
**Severidade:** Minor · **Prioridade:** Medium

**Ambiente registrado:** Windows 10 Pro 22H2; Chrome 154.0.8037.98 (64-bit)

**Pré-condições:** Controlled candidate/recruiter chats.

**Passos:**

1. Log in as candidate.
2. Open active or archived chat.
3. Inspect actions.
4. Repeat as recruiter.

**Resultado obtido:** Archive/Unarchive and Delete are available, but no Favourite action is present.

**Resultado esperado:** Both roles should be able to mark a chat as favourite and retain that state.

## HUNT-32 — User cannot create or switch to a second role

**Plataforma:** Web  
**Severidade:** Major · **Prioridade:** High

**Ambiente registrado:** Windows 10 Pro 22H2; Chrome 154.0.8037.98 (64-bit)

**Pré-condições:** Account with only one role created.

**Passos:**

1. Log in.
2. Open Profile.
3. Open Account settings if applicable.
4. Look for create-missing-role option.
5. Check for role switch control.

**Resultado obtido:** No option to create the second role or switch between Candidate and Recruiter is available.

**Resultado esperado:** User should be able to create the missing role and switch between Candidate and Recruiter profiles.

## HUNT-33 — Telegram and Signal links are missing from the footer

**Plataforma:** Web  
**Severidade:** Minor · **Prioridade:** Medium

**Ambiente registrado:** Windows 10 Pro 22H2; Chrome 154.0.8037.98 (64-bit)

**Pré-condições:** Open Huntd website.

**Passos:**

1. Open Huntd website.
2. Scroll to footer.
3. Review social links.
4. Check for Telegram and Signal.

**Resultado obtido:** LinkedIn, Facebook, Twitter and Instagram are present, but Telegram and Signal are missing.

**Resultado esperado:** Footer should include all expected social links, including Telegram and Signal.

## HUNT-34 — Company links do not open vacancies in a new tab

**Plataforma:** Web  
**Severidade:** Minor · **Prioridade:** Medium

**Ambiente registrado:** Windows 10 Pro 22H2; Chrome 154.0.8037.98 (64-bit)

**Pré-condições:** Open Web3 companies page.

**Passos:**

1. Open Web3 companies page.
2. Locate Coinbase.
3. Click logo.
4. Click company name.
5. Observe navigation.

**Resultado obtido:** Logo opens vacancies in the current tab and the company name is not clickable.

**Resultado esperado:** Both logo and company name should open company vacancies in a new tab.
