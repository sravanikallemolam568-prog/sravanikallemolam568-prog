

import { Github, ExternalLink, GitFork, Star } from "lucide-react";
import { Reveal } from "./Reveal";
import { Section } from "./Section";

export function GithubSection() {
  return (
    <Section
      id="github"
      eyebrow="GitHub"
      title="My GitHub"
      description="Explore my projects, experiments, and development work on GitHub."
    >
      <Reveal>
        <div className="glass-card lift p-6 sm:p-8">
          <div className="flex flex-col gap-6 sm:flex-row sm:items-center sm:justify-between">
            <div className="flex items-start gap-4">
              <span className="grid size-12 shrink-0 place-items-center rounded-xl bg-secondary text-primary">
                <Github size={24} />
              </span>

              <div>
                <h3 className="font-display text-xl font-semibold">
                  AI & ML Developer
                </h3>

                <p className="mt-2 text-sm text-muted-foreground">
                  I use GitHub to build, manage, and share my projects,
                  experiments, and AI-based applications.
                </p>
              </div>
            </div>

            <a
              href="https://github.com/YOUR-GITHUB-USERNAME"
              target="_blank"
              rel="noreferrer"
              className="inline-flex w-fit items-center gap-2 rounded-full border border-border px-5 py-2.5 text-sm font-semibold transition-colors hover:border-primary"
            >
              <Github size={16} />
              Visit GitHub
              <ExternalLink size={14} />
            </a>
          </div>

          <div className="mt-6 grid gap-4 sm:grid-cols-3">
            <div className="rounded-xl border border-border p-4">
              <GitFork size={18} className="text-primary" />
              <h4 className="mt-3 font-semibold">Projects</h4>
              <p className="mt-1 text-sm text-muted-foreground">
                AI, ML and web development projects
              </p>
            </div>

            <div className="rounded-xl border border-border p-4">
              <Star size={18} className="text-primary" />
              <h4 className="mt-3 font-semibold">Learning</h4>
              <p className="mt-1 text-sm text-muted-foreground">
                Learning through practical coding and experiments
              </p>
            </div>

            <div className="rounded-xl border border-border p-4">
              <Github size={18} className="text-primary" />
              <h4 className="mt-3 font-semibold">Open Source</h4>
              <p className="mt-1 text-sm text-muted-foreground">
                Sharing useful projects and development work
              </p>
            </div>
          </div>
        </div>
      </Reveal>
    </Section>
  );
}
