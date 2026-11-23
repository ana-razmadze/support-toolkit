# Escalation Playbook

A simple guide for when and how to pass a support ticket to someone else. Written for a pretend online shop, BrightCart.

**Goal:** the customer gets a fast answer, and nobody has to ask the same question twice.

## 1. When to escalate

Escalate if **any** of these is true:

- The customer lost money (double charge, fraud, big refund)
- The problem affects many customers (for example, the website is down)
- The ticket is close to missing the deadline (SLA) and I cannot fix it myself
- The customer is asking for something I am not allowed to approve
- The customer mentions a lawyer, the press, or the bank (chargeback)
- The same problem came back 3 times

**Do not escalate** if the answer is in the knowledge base, or if I just need to ask the customer one more question.

## 2. Levels

| Level | Who | Example | Reply time |
|---|---|---|---|
| L1 | Support agent | Password, order status, simple refund | 24 hours |
| L2 | Senior agent / Team lead | Angry customer, refund over $200, repeat problem | 4 hours |
| L3 | Specialist team (payments, tech, warehouse) | Payment errors, bugs, lost packages | 1 business day |
| L4 | Manager | Legal, press, safety, large outage | 1 hour |

## 3. Before I escalate: checklist

- [ ] I read the whole ticket history
- [ ] I tried the steps in the knowledge base
- [ ] I have the order number and customer email
- [ ] I have screenshots or photos if needed
- [ ] I told the customer what is happening

## 4. Escalation note (copy this format)

```
SUMMARY: One sentence. What is the problem?
CUSTOMER: Name, email, order number
IMPACT: Money lost? How many customers? Deadline?
WHAT I TRIED: Step 1, step 2, step 3
WHAT I NEED: A clear request. "Please check payment BC-4821 and approve refund."
DEADLINE: Date and time
```

**Example:**

```
SUMMARY: Customer was charged twice for the same order.
CUSTOMER: Maria K., maria@example.com, order BC-4821
IMPACT: $89 charged twice. Customer wrote 2 times already.
WHAT I TRIED: Checked order system, only one order exists. Asked the customer for a bank screenshot, received it.
WHAT I NEED: Payments team to confirm the double charge and refund $89.
DEADLINE: Tomorrow 12:00. Customer is waiting.
```

## 5. What I tell the customer

Use [template 6](../reply-templates/templates.md) and always say:
1. Who is looking at the case now
2. When they will get an answer
3. That they do not need to repeat their story

## 6. After I escalate

1. Set a reminder to check the ticket at the deadline.
2. If there is no answer by the deadline, ask again in the team chat, and tell the customer.
3. When the case is closed, write to the customer and say sorry if we were slow.
4. Add a note: **why did this happen?**

## 7. Learn from it

Every month, I look at all escalated tickets and ask:

- Did we need to escalate, or could L1 solve it with better training?
- Is there a missing knowledge base article?
- Is the same bug or process problem causing many tickets?

Then I write the article, fix the process, or report the bug. Fewer escalations = faster answers = happier customers.

## Flow

```
Ticket comes in
      |
Can I solve it with the knowledge base? -- Yes --> Solve, reply, close
      | No
Is it money, many customers, legal, or urgent? -- Yes --> Escalate with a note
      | No
Ask the customer for what is missing, then try again
      |
Still stuck after 2 tries? --> Escalate
```
