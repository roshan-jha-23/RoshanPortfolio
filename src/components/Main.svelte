<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "Whisper Wire",
            icon: "fa-solid fa-envelope",
            description:
                "Whisper Wire is an innovative application made using Next.js. It allows you to send messages to anyone following the link while keeping your identity secret. It uses modern tools such as NodeMailer for sending mail, Bcryptjs for hashing passwords, Zod for validations and checks, and MongoDB for the database. It also leverages Shadcn components and Tailwind CSS for inline styling.",
        },
        {
            name: "CoderStop",
            icon: "fa-solid fa-code",
            description:
                "CoderStop is a dynamic platform for coders, built with Next.js and AcertinityUI, an open-source component library. This app serves as a one-stop platform for coders worldwide, allowing them to interact, make friends, and chat with other coders. It also provides features to view their current positions and see coders across the globe. Various API endpoints are used to help with GitHub, Codeforces, and LeetCode integration. Tools used include Shadcn, Zod, MongoDB, Redis, Auth.js, Next.js, JWT, Bcrypt, and Sender.",
        },
        {
            name: "Phone-Case-Cobra",
            icon: "fa-solid fa-snake",
            description:
                "Phone-Case-Cobra is an app made using Prisma for the database and Kinde for authentication. Zod is used for validation, and Stripe handles payments and webhooks. The app offers a comprehensive solution for phone case purchases with secure transactions.",
        },
        {
            name: "Youtube-Twitter",
            icon: "fa-brands fa-youtube",
            description:
                "Youtube-Twitter combines the functionalities of both platforms, allowing users to share and discuss videos and tweet their thoughts. It leverages Cloudinary for effortless image and video uploads, MongoDB for scalable data storage, Bcrypt for password and credential hashing for user protection, and Multer for smooth file handling. The front end is developed using Vite, a fast build tool for web development.",
        },
        {
            name: "MusicAcedmia",
            icon: "fa-solid fa-music",
            description:
                "MusicAcedmia is an app for a music school where music is taught. It is made using AI Certainty and Next.js, incorporating some components from Shadcn.",
        },
        {
            name: "Chat App",
            icon: "fa-solid fa-comments",
            description:
                "The Chat App is a real-time chat application made using Pusher.js, Redis, and the concept of Socket.io. It includes Zod for validation and Next.js for development. Users can add friends and have real-time conversations.",
        },
    ];

    let benefits = [
        {
            metric: "10x",
            name: "Self-Taught Developer with a Foundation in Java",
            description:
                "I embarked on my coding journey by delving into Java for data structures and algorithm problem-solving. As my passion for programming grew, I expanded my skill set to include HTML, CSS, and JavaScript, gradually evolving into a well-rounded developer. I've continued to explore various technologies, from frontend frameworks to backend programming, design, and cloud services. My journey is a testament to my love for creativity and problem-solving in the realm of innovative online experiences.",
        },
        {
            name: "Code Enthusiast on a Learning Journey",
            description:
                "I am a full-stack developer passionate about coding and technology. While I may be relatively new to the industry, I am enthusiastic about tackling challenges and continuously expanding my skill set. My focus is on creating robust solutions and enhancing user experiences across the digital landscape. Eager to contribute, learn, and grow as a developer.",
        },
        {
            name: "Effective Communicator and Collaborator",
            description:
                "While I may lean towards introversion, my commitment to clear and constructive communication remains unwavering. I thrive in fostering transparent dialogues and building strong connections within a team. Despite my introverted nature, I become a people person in the context of work, allowing me to contribute effectively and enhance productivity in any collaborative environment.",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-violet-300">Roshan</span> Jha,
                <br /> A Full Stack
                <span class="poppins text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-green-400"> favorite tech</span> includes Java(for DSA) and for Dev JavaScript
                (React.js, NEXT.JS or SvelteKit), TailwindCSS, Node.js + Express.js , PostgreSQL & MongoDB
                or Firebase/Firestore!
            </p>
            <a href="https://twitter.com/roshan_jha_23" target="_blank">
                <button class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950">
                    <div class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200" />
                    <h4 class="relative z-9">Get in touch &rarr;</h4>
                </button>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src="/images/profile.png"
                alt="Profile Picture"
                class="object-cover z-[2] max-h-[70vh]"
            />
        </div>
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                A few of my endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>
        <a
            href="#"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
        >
            <i class="fa-regular fa-circle-play" />
            <p>Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            {#each steps as step}
                <Step {step}>
                    <p>
                        This contri was made to SurrealDB <strong class="text-violet-400">React.js, SurrealDB & Node.js + Express.js!</strong> A curated list of SurrealDB resources, tools, utilities, and applications.
                    </p>
                </Step>
            {/each}
            <div>
                <strong><h1>And More To Come.....</h1></strong>
            </div>
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <div class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">
            <h6 class="text-large sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me
            </h3>
        </div>
        <div
            class="grid grid-cols-1 lg:grid-cols-2 gap-12 md:gap-20 lg:gap-24"
        >
            <div
                class="p-6 flex flex-col gap-6 sm:gap-8 md:gap-10 lg:gap-14 rounded-lg shadow-lg"
            >
                <h5 class="font-semibold text-2xl sm:text-3xl md:text-4xl">
                    Where <span class="poppins text-violet-400">it began.</span>
                </h5>
                <div
                    class="grid grid-cols-1 md:grid-cols-2 md:gap-8 md:divide-x-2 md:divide-solid md:divide-white gap-6 sm:gap-8 md:gap-10 lg:gap-14"
                >
                    {#each benefits as benefit}
                        <div
                            class="flex flex-col gap-4 md:gap-6 lg:gap-8 text-center md:text-left"
                        >
                            {#if benefit.metric}
                                <h6
                                    class="text-lg sm:text-xl md:text-2xl font-semibold"
                                >
                                    {benefit.metric}
                                </h6>
                            {/if}
                            <p class="font-semibold">{benefit.name}</p>
                            <p>{benefit.description}</p>
                        </div>
                    {/each}
                </div>
            </div>
            <div class="shadow-xl rounded-lg h-[70vh]">
                <img
                    src="/images/profile.png"
                    alt="Profile Picture"
                    class="object-cover w-full h-full rounded-lg"
                />
            </div>
        </div>
    </section>
</main>

<style>
    .blueShadow {
        box-shadow: 0px 0px 18px -4px #c4b5fd;
    }

    .blueShadow h4 {
        z-index: 9;
    }

    .poppins {
        font-family: "Poppins", sans-serif;
    }

    .pr-14 {
        padding-right: 3.5rem;
    }
</style>
