# Contributing to bce

Teşekkürler — proje ile katkıda bulunmayı düşündüğün için memnunuz. Bu dosya, katkı sürecini, beklentileri ve kuralları açıklar. Projeye katkı sağlamadan önce lütfen aşağıdaki maddeleri okuyup kabul ettiğini varsayacağız.

## Özet
- Bireysel ve akademik araştırma/deney amaçlı kullanım serbesttir.
- Ticari ticarileşme (satış, abonelik, OEM, white‑label, SaaS vb.) durumunda yazılı izin ve lisans/royalty (brüt satış gelirinin %0,5) uygulanır.
- Dış katkılar kabul edilebilir; katkılar ticarileşme veya yatırım durumunda önem derecesine göre tazmin edilebilir. Katkı kabul şartları ve tazminat politikası `CONTRIBUTING.md` ve gerekirse ayrı bir sözleşme/CLA ile düzenlenecektir.
- Projeye katkı yapmadan önce bu dosyayı ve `LICENSE_SUMMARY.md` içeriğini okuyun.

## Davranış Kuralları (Code of Conduct)
Bu projeye katkıda bulunurken profesyonel, saygılı ve kapsayıcı davranış beklenir. Kaba, ayrımcı veya taciz edici davranış kabul edilemez. Gerekirse ayrıca bir CODE_OF_CONDUCT.md dosyası oluşturulabilir.

## Katkı Türleri
- Hata raporları (bug)
- Özellik istekleri (feature request)
- Küçük düzeltmeler (typo, dokümantasyon)
- Kod katkıları (PR)
- Testler ve CI iyileştirmeleri
- Güvenlik bildirimleri (özel iletilmeli; bakınız "Güvenlik")

## Issue açma
- Mevcut issue'ları kontrol edin; aynı sorunu tekrar açmayın.
- Açarken:
  - Başlık kısa ve açıklayıcı olsun.
  - Adımlar yeniden üretilebilir şekilde verilsin.
  - Beklenen ve gözlemlenen davranış açıkça yazılsın.
  - Sistem/çevre bilgileri (örn. Python/Node versiyonu, ilgili paketler) ekleyin.
- "feature request" açarken kullanım senaryosu, alternatif çözümler ve arzu edilen API/UX örnekleri ekleyin.

## Çalışma ortamı / Local development
- Fork → feature branch (branch ismi: feat/<kısa-açıklama> veya fix/<kısa-açıklama>).
- Commit mesajları için Conventional Commits önerilir: feat:, fix:, docs:, chore: vb.
- Kod stili: proje köküne eklenecek .editorconfig / linter kurallarına uyun. (Varsa proje stil rehberine link eklenecek.)
- Yeni kod ekliyorsanız ilgili testleri ekleyin veya mevcut testleri güncelleyin.

## Pull Request (PR) kuralları
- Her PR tek konuda olsun.
- PR açıklamasında:
  - Ne yapıldığı ve neden yapıldığı,
  - İlgili issue numarası (örn. "Resolves #123"),
  - Test talimatları ve local olarak nasıl doğrulanacağı,
  - Gerekliyse performans/benchmark etkileri.
- PR checklist (en az):
  - [ ] Kod lint'ten geçti
  - [ ] Tüm testler geçti
  - [ ] Dokümantasyon güncellendi (gerekliyse)
  - [ ] OFFSET/SECRET bilgisi commit'e dahil değil
  - [ ] Lisans atıfı/HEADER eklendi
- En az bir maintainer onayı gerektirir; kritik değişiklikler için 2 onay istenebilir.

## Test & CI
- PR'lar CI tarafından otomatik testlenir. CI hatalarını düzeltmeden PR merge edilmez.
- Yeni özelliklerle beraber birim/integrasyon testleri ekleyin.
- Test verileri kişisel veri (PII) içermemelidir.

## Kod kalitesi ve güvenlik
- Gizli anahtarlar/şifreler asla commit edilmez.
- Güvenlik açıklarını bulduğunuzda lütfen public issue açmayın; `iletisimahmetkahraman@gmail.com` adresine özel olarak bildirin — rapid response ve koordinasyon yapılacaktır.
- Üçüncü taraf kütüphane lisans uyumluluğuna dikkat edin; telif/uyumluluk sorunları olursa maintainer ile görüşün.

## Lisans, IP ve CLA
- Bu proje özel/ticari lisans kapsamındadır. Katkı sağladığınız kod veya dokümantasyonun sahipliği ve kullanım hakları hakkında proje yöneticileriyle (Licensor) görüşülüp açık bir anlaşma yapılması gerekebilir.
- Eğer katkı kabul edilirse, katkının niteliğine göre bir CLA (Contributor License Agreement) veya IP devri/agreement imzalanması istenebilir.
- Proje ticarileştiğinde katkılara yapılacak ödemeler veya paylaşımlar, katkının önemine ve önceden üzerinde anlaşılan koşullara göre belirlenecektir. Bu politika ayrı bir agreement ile netleştirilecektir.

## Attribution (Atıf)
- Ticari veya dağıtılan sürümlerde atıf zorunludur: ör. "Contains Behavioral Consciousness Engine (BCE) — © Ahmet Kahraman".
- Kaynak dosyalarına kısa lisans başlığı (`LICENSE_HEADER.txt`) eklenmelidir.

## Ödemeler ve tazminat
- Proje yatırım alır veya ticarileşirse, dış katkılara ödemeler yapılabilir. Bu konuda karar ve hesaplama proje sahipleri tarafından yapılır; katkı sahipleri ile sözlü değil yazılı anlaşma (contract) yapılacaktır.

## Denetim ve kayıtlar
- Kullanıcı/satış verileri üzerinden royalty hesaplanması, raporlama ve denetim talepleri sözleşmede belirtilecektir. Katılımcıların proje ile ilgili ticari verileri paylaşma yükümlülüğü yalnızca taraflarca kararlaştırıldığında geçerlidir.

## İletişim
- Ticari lisans ve izin talepleri: iletisimahmetkahraman@gmail.com
- Güvenlik bildirimleri (kamuya açık değil): iletisimahmetkahraman@gmail.com (başlığa "SECURITY" ekleyin)

```markdown
# Contributing to bce

Thank you — we're glad you're considering contributing. This file explains the contribution process, expectations, and rules. By contributing you agree to the guidelines below.

## Summary
- Personal and academic research/experimentation is permitted without prior permission.
- Commercialization (sales, subscriptions, OEM, white‑label, SaaS, etc.) requires written permission and is subject to licensing/royalty (0.5% of gross sales revenue).
- External contributions may be accepted; if the project is commercialized or receives funding, contributors may be compensated based on contribution significance. Contribution acceptance, compensation terms, and IP arrangements will be defined in CONTRIBUTING.md and, where necessary, in a separate agreement/CLA.
- Read this file and LICENSE_SUMMARY.md before contributing.

## Code of Conduct
Contributors are expected to act professionally, respectfully, and inclusively. Abusive, discriminatory, or harassing behavior is not tolerated. A separate CODE_OF_CONDUCT.md can be added if desired.

## Types of contributions
- Bug reports
- Feature requests
- Small fixes (typos, docs)
- Code contributions (PRs)
- Tests and CI improvements
- Security reports (see Security section)

## Filing an issue
- Check existing issues before opening a new one.
- Use a clear, descriptive title.
- Provide reproducible steps, expected vs. actual behavior.
- Add environment details (e.g., Python/Node versions, relevant packages).
- For feature requests include use case, alternatives, and desired API/UX.

## Local development
- Fork → feature branch (branch naming: feat/<short-desc> or fix/<short-desc>).
- Use Conventional Commits where possible: feat:, fix:, docs:, chore:, etc.
- Follow project style guidelines (.editorconfig / linters). Add tests for new code or update existing tests.
- Ensure secrets are not committed.

## Pull Request (PR) guidelines
- Keep each PR focused on a single topic.
- PR description should include:
  - What and why,
  - Related issue number (e.g., "Resolves #123"),
  - How to test locally,
  - Any performance/benchmark notes if relevant.
- PR checklist (minimum):
  - [ ] Lint passes
  - [ ] All tests pass
  - [ ] Documentation updated if needed
  - [ ] No secrets or sensitive data in commits
  - [ ] License header added where appropriate
- At least one maintainer approval is required; critical changes may need two approvals.

## Tests & CI
- PRs are validated by CI. Fix CI failures before merge.
- Add unit/integration tests for new features.
- Test data must not include personal data (PII).

## Code quality & security
- Never commit secrets (API keys, passwords).
- Report security vulnerabilities privately: iletisimahmetkahraman@gmail.com (do not open public issues).
- Check third‑party dependency licenses for compatibility; consult maintainers if unsure.

## License, IP, and CLA
- This project is covered by a proprietary/commercial license. Contribution acceptance may require a CLA or specific IP assignment/license terms.
- If contributions are accepted, maintainers will discuss IP rights and any compensation before merging significant work.
- Contributions do not automatically entitle the contributor to royalties unless explicitly agreed in writing.

## Attribution
- Attribution is required in distributed/commercial releases, e.g.: "Contains Behavioral Consciousness Engine (BCE) — © Ahmet Kahraman".
- Add the project license header to source files as appropriate (LICENSE_HEADER.txt).

## Payments and compensation
- If the project receives funding or commercializes, contributors may be paid based on contribution importance and prior agreement. Any payment arrangements will be documented in a written contract.

## Audit & records
- Royalty calculation, reporting, and audit procedures will be defined in license agreements. Contributors are not required to share commercial records unless explicitly agreed between parties.

## Contact
- Commercial licensing and permission requests: iletisimahmetkahraman@gmail.com
- Security reports (confidential): iletisimahmetkahraman@gmail.com — include "SECURITY" in the subject.

```

