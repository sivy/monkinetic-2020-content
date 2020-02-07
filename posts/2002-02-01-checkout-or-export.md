date: 2002-02-01
slug: checkout-or-export
title: Checkout or Export?
---
CVS question: when doing a checkout for the purpose of building a project on a testing platform, is it preferred to do a `` checkout ``, and ignore the CVS files that come along, or an explicit `` export `` to get only the source?

I think for testing purposed (we'll run this a lot more than deployment) `` checkout `` will work - I'd rather not have to be limited to a particular tag or date, I only want the most recent. But I'm open to solutions to this problem.