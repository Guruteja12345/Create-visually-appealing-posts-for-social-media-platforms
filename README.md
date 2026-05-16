export default function GitHubStyleSocialPosts() {
  const posts = [
    {
      title: "Internship Opportunity",
      subtitle: "Build Skills • Gain Experience • Grow Professionally",
      description:
        "Join our internship program and work on real-world projects with industry mentors.",
      cta: "Apply Now",
    },
    {
      title: "Career Growth Starts Here",
      subtitle: "Learn From Experts",
      description:
        "Enhance your technical and communication skills through hands-on experience.",
      cta: "Start Today",
    },
    {
      title: "Future Ready Internship",
      subtitle: "Practical Learning Experience",
      description:
        "Gain industry exposure and strengthen your resume with professional projects.",
      cta: "Join Us",
    },
  ];

  return (
    <div className="min-h-screen bg-gray-100 p-8">
      <div className="max-w-7xl mx-auto">
        <h1 className="text-4xl font-bold text-center text-gray-900 mb-4">
          GitHub Style Social Media Posts
        </h1>
        <p className="text-center text-gray-600 mb-10 text-lg">
          Professional internship promotional templates for Instagram & LinkedIn
        </p>

        <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          {posts.map((post, index) => (
            <div
              key={index}
              className="bg-white rounded-3xl shadow-xl overflow-hidden border border-gray-200 hover:scale-105 transition-transform duration-300"
            >
              <div className="bg-gray-900 p-5 text-white">
                <div className="flex items-center gap-2 mb-3">
                  <div className="w-3 h-3 rounded-full bg-red-500"></div>
                  <div className="w-3 h-3 rounded-full bg-yellow-400"></div>
                  <div className="w-3 h-3 rounded-full bg-green-500"></div>
                </div>

                <div className="font-mono text-sm text-green-400">
                  github/social-post-template
                </div>
              </div>

              <div className="p-6">
                <div className="inline-block px-3 py-1 rounded-full bg-gray-200 text-sm font-medium text-gray-700 mb-4">
                  Internship Program
                </div>

                <h2 className="text-2xl font-bold text-gray-900 mb-2">
                  {post.title}
                </h2>

                <p className="text-blue-600 font-semibold mb-4">
                  {post.subtitle}
                </p>

                <p className="text-gray-600 leading-relaxed mb-6">
                  {post.description}
                </p>

                <button className="w-full bg-gray-900 hover:bg-black text-white py-3 rounded-2xl font-semibold transition-colors duration-300">
                  {post.cta}
                </button>
              </div>

              <div className="border-t border-gray-200 px-6 py-4 bg-gray-50 flex justify-between text-sm text-gray-500">
                <span>#Internship</span>
                <span>#CareerGrowth</span>
                <span>#GitHubStyle</span>
              </div>
            </div>
          ))}
        </div>

        <div className="mt-12 bg-white rounded-3xl shadow-lg p-8 border border-gray-200">
          <h2 className="text-2xl font-bold text-gray-900 mb-4">
            GitHub Deployment Instructions
          </h2>

          <ol className="list-decimal list-inside text-gray-700 space-y-3">
            <li>Create a new GitHub repository.</li>
            <li>Upload this React component.</li>
            <li>Use Vite or Next.js setup.</li>
            <li>Push the code to GitHub.</li>
            <li>Enable GitHub Pages for deployment.</li>
          </ol>

          <div className="mt-6 p-4 bg-gray-100 rounded-2xl font-mono text-sm text-gray-800 overflow-x-auto">
            git init
            <br />
            git add .
            <br />
            git commit -m "Add social media post templates"
            <br />
            git branch -M main
            <br />
            git remote add origin YOUR_GITHUB_REPO
            <br />
            git push -u origin main
          </div>
        </div>
      </div>
    </div>
  );
}
